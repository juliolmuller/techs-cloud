<h1 align="center">
  :cloud: Interactive 3D Tech Stack Cloud
</h1>

<p align="center">
  <a href="#trophy-lessons-learned">Lessons Learned</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#rocket-technologies--resources">Technologies</a>
</p>

<p align="center">
  <img src="https://img.shields.io/static/v1?labelColor=000000&color=012233&label=created%20at&message=october%202026" alt="Creation Date" />

  <img src="https://img.shields.io/github/last-commit/juliolmuller/techs-cloud?label=updated%20at&labelColor=000000&color=012233" alt="Update Date" />

  <img src="https://img.shields.io/static/v1?labelColor=000000&color=012233&label=PRs&message=welcome" alt="Pull Requests Welcome" />

  <img src="https://img.shields.io/github/license/juliolmuller/techs-cloud?labelColor=000000&color=012233" alt="Project License" />
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/dc1b914e-15fb-4994-959e-e0d4e193a26f" alt="Demo" />
</p>

This project is a browser-based, interactive 3D geoid of my tech stack. It scatters 80+ logos across a sphere using a Fibonacci distribution and keeps them orbiting with depth-based scale and opacity. Everything runs on vanilla HTML, CSS, and JavaScript, without WebGL or frameworks. Drag to spin the cloud with a mouse or touch; hover an icon to reveal its name and slow that item down.

[Check out the page running!](https://juliolmuller.github.io/techs-cloud)

## :trophy: Lessons Learned

- Distributing points evenly on a sphere with the Fibonacci golden-ratio spiral.
- Faking a 3D scene with CSS `perspective` and per-frame `transform`, `opacity`, and `z-index`, without Three.js.
- Mapping a Z coordinate to scale, fade, stacking order, and `pointer-events` so only the front hemisphere is interactive.
- Drag-and-inertia physics: velocity from mouse/touch delta, friction damping on release.
- Latitude-based rotation speeds (faster near the poles) plus a hover slowdown lerp.
- Subtle per-icon sine float so the geoid doesn't look rigid.
- Loading logos from Devicon, SVGL, and Simple Icons with `onerror` fallbacks and invert filters for dark backgrounds.
- Softening the viewport edges with a radial CSS mask.

## :rocket: Technologies & Resources

- HTML & CSS
- JavaScript (vanilla)
- [CSS 3D Transforms](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-function/perspective)
- [Devicon](https://devicon.dev/)
- [SVGL](https://svgl.app/)
- [Simple Icons](https://simpleicons.org/)

---

:star2: Feel free to submit pull requests to improve this project.
