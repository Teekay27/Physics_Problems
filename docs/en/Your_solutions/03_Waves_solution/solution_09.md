## 9. Damped Oscillator

### Problem

For the damped harmonic oscillator:

$$
m \frac{d^2 x}{dt^2} + b \frac{dx}{dt} + k x = 0
$$

Create an interactive animation with a slider for $b$ showing:
- Underdamped
- Critically damped
- Overdamped

Include:
- Graph of $x(t)$
- Phase portrait $(x, v)$

---

## 🧠 1. General Solution

Define:

$$
\gamma = \frac{b}{2m}, \quad \omega_0 = \sqrt{\frac{k}{m}}
$$

---

### Underdamped ($\gamma < \omega_0$)

$$
x(t) = A e^{-\gamma t} \cos(\omega_d t + \phi)
$$

$$
\omega_d = \sqrt{\omega_0^2 - \gamma^2}
$$

---

### Critically Damped ($\gamma = \omega_0$)

$$
x(t) = (A + Bt)e^{-\gamma t}
$$

---

### Overdamped ($\gamma > \omega_0$)

$$
x(t) = A e^{r_1 t} + B e^{r_2 t}
$$

---

## 🧠 2. Classification

- Underdamped: oscillates with decay  
- Critically damped: fastest return, no oscillation  
- Overdamped: slow return, no oscillation  

---

## 🧠 3. Numerical Solution (RK4)

We rewrite as system:

$$
\dot{x} = v
$$

$$
\dot{v} = -\frac{b}{m}v - \frac{k}{m}x
$$

---



<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Damped Oscillator</title>
<style>
canvas { border:1px solid black; margin:10px; }
</style>
</head>
<body>

<h3>Damped Oscillator Simulation</h3>

<label>b:
<input type="range" min="0" max="10" step="0.1" value="1" id="bSlider">
</label>
<span id="bVal"></span>

<p id="type"></p>

<canvas id="xt" width="600" height="250"></canvas>
<canvas id="phase" width="600" height="250"></canvas>

<script>
const xt = document.getElementById("xt").getContext("2d");
const ph = document.getElementById("phase").getContext("2d");

let m = 1, k = 10, dt = 0.02;

function accel(x,v,b){
    return (-b*v - k*x)/m;
}

function rk4(x,v,b){
    let k1x=v;
    let k1v=accel(x,v,b);

    let k2x=v+0.5*dt*k1v;
    let k2v=accel(x+0.5*dt*k1x, v+0.5*dt*k1v,b);

    let k3x=v+0.5*dt*k2v;
    let k3v=accel(x+0.5*dt*k2x, v+0.5*dt*k2v,b);

    let k4x=v+dt*k3v;
    let k4v=accel(x+dt*k3x, v+dt*k3v,b);

    x += dt*(k1x+2*k2x+2*k3x+k4x)/6;
    v += dt*(k1v+2*k2v+2*k3v+k4v)/6;

    return [x,v];
}

function classify(b){
    let gamma=b/(2*m);
    let w0=Math.sqrt(k/m);

    if(gamma < w0) return "Underdamped";
    if(gamma === w0) return "Critically damped";
    return "Overdamped";
}

function draw(){
    let b = parseFloat(document.getElementById("bSlider").value);
    document.getElementById("bVal").innerText = b.toFixed(2);
    document.getElementById("type").innerText = classify(b);

    xt.clearRect(0,0,600,250);
    ph.clearRect(0,0,600,250);

    let x=1, v=0;

    xt.beginPath();
    ph.beginPath();

    for(let i=0;i<400;i++){
        let px=i*1.5;
        let py=125 - x*80;

        if(i===0) xt.moveTo(px,py);
        else xt.lineTo(px,py);

        let phx = 300 + x*100;
        let phy = 125 - v*20;

        if(i===0) ph.moveTo(phx,phy);
        else ph.lineTo(phx,phy);

        [x,v] = rk4(x,v,b);
    }

    xt.stroke();
    ph.stroke();
}

document.getElementById("bSlider").oninput = draw;
draw();
</script>

</body>
</html>