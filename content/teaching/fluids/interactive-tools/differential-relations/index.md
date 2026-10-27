---
title: "Differential Relations & Vorticity 🌀"
layout: "simple"
showDate: false
showReadingTime: false
showWordCount: false
build:
  list: never
---

{{< katex >}}

<div class="project-img">
<video src="/img/teaching/differential-relations-video-1.mp4" class=" rounded-lg" autoplay loop muted playsinline onclick="openMediaLightbox(this)"></video>
</div>

The video above zooms into a tiny fluid element \\( dx \times dy \\). Instead of a big control volume, we look at what one small square does as it moves with the flow, and it turns out it can only do four things: **translate**, **rotate**, **stretch** (linear strain) and **shear** (angular deformation). In a real flow all four happen at once, but we can "divide and conquer" by looking at each one separately. The <span style="color: #c0392b; font-weight: bold;">red arcs</span> \\( d\alpha \\) and \\( d\beta \\) show how much each edge turns. If both edges turn the same way, the element is rotating: \\( \omega_z = \frac{1}{2}\left(\frac{\partial v}{\partial x} - \frac{\partial u}{\partial y}\right) \\). If they turn towards each other, the right angle closes and it's shear: \\( \dot\gamma_{xy} = \frac{\partial u}{\partial y} + \frac{\partial v}{\partial x} \\). Note that none of these motions change the area of the element, only \\( \nabla \cdot \vec V = \frac{\partial u}{\partial x} + \frac{\partial v}{\partial y} \\) can do that, which is zero for incompressible flow.

<div class="project-img">
<video src="/img/teaching/differential-relations-video-2.mp4" class=" rounded-lg" autoplay loop muted playsinline onclick="openMediaLightbox(this)"></video>
</div>

The 2nd video compares two flows where the fluid moves in circles. Each cross (and the 🙂) is a tiny paddle wheel, think of it as a "vorticity meter". On the left (forced vortex, \\( u_\theta = \Omega r \\)), the paddles spin as they go around, so the flow is **rotational** with vorticity \\( \zeta_z = 2\Omega \\). On the right (free vortex, \\( u_\theta = K/r \\)), the paddles go around but always point the same way, the smiley face never turns upside down, so the flow is **irrotational** with \\( \zeta_z = 0 \\). Remember vorticity measures whether the fluid element *spins*, not whether its path is curved.

<div class="project-img">
<video src="/img/teaching/differential-relations-video-3.mp4" class=" rounded-lg" autoplay loop muted playsinline onclick="openMediaLightbox(this)"></video>
</div>

The 3rd video is the flip side: simple shear (Couette) flow between a fixed plate and a moving plate, \\( u = U\frac{y}{h} \\). The streamlines are perfectly straight, but the top of the element moves faster than the bottom, so only its vertical edge tilts. That makes the flow **rotational**, \\( \zeta_z = -\frac{U}{h} \\) (clockwise), and the element is also shearing, \\( \dot\gamma_{xy} = \frac{U}{h} \\). In fact shear = rigid rotation (half the angle) + pure strain, which is what the small boxes at the bottom show.

**Quick tip:** for linear profiles like this one (or the sleeve bearing in Problem 1), the profile is literally \\( y = mx + c \\). The two no-slip walls give you the two points, and the slope \\( m = \frac{\partial u}{\partial y} = \frac{\Delta u}{h} \\) is all you need for both \\( \dot\gamma_{xy} \\) and \\( \zeta_z \\).

<!-- Source Code: [Google Colab](link here) -->