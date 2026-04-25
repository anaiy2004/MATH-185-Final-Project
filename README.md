# MATH 185 Final Project

Coding tool for my Math 185 final project on conformal maps and 2D fluid dynamics. Renders flow past a Joukowski airfoil by transporting the flow past an offset cylinder through `w = z + a^2/z`.

[Online Demo (Easiest)](https://anaiy2004.github.io/MATH-185-Final-Project/joukowski.html)

## Run it locally

Simply download `joukowski.html` and open it.

```
git clone https://github.com/anaiy2004/MATH-185-Final-Project.git
open MATH-185-Final-Project/joukowski.html
```

## what it does

Two canvases side by side: cylinder on the left (z-plane), airfoil on the right (w-plane). Same flow in both, the right one is just the left with `J` applied. Sliders for thickness, camber, angle of attack, freestream speed. Checkbox toggles the Kutta condition.

Streamlines: Sample psi on a 240x200 grid, Run marching squares to get level sets, then draw each segment in both canvases (the w-plane version just maps the endpoints through J).
