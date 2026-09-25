---
title: "Hydrostatic Pressure on Curved Plate ⚓"
layout: "simple"
showDate: false
showReadingTime: false
showWordCount: false
build:
  list: never
---

{{< katex >}}

<div class="project-img">
<video src="/img/teaching/pressure-animation.mp4" class=" rounded-lg" autoplay loop muted playsinline onclick="openMediaLightbox(this)"></video>
</div>

The video above shows how we deal with pressure on curved surface, we basically "divide and conqure" by decoupling the \\( x \\) and \\( y \\) components. For horizontal component \\( P_x \\), we can treat it as if it's a vertical plate.  \\( CP = CG \\) at mid height and \\( P_x = \rho g h_{CG}\\). For the vertical component \\( P_y \\), it's even easier, we just need the weight of the fluids above \\( P_y= \rho g \\) <del>V</del>\\( _{above} \\).

<div class="project-img">
<video src="/img/teaching/pressure-inverted-animation.mp4" class=" rounded-lg" autoplay loop muted playsinline onclick="openMediaLightbox(this)"></video>
</div>

The 2nd video shows a inverted scenario, remember pressure from liquid is always acting on a surface no matter the geometry. For these upside down ish scenario, we use a virtual/imaginary water method for \\( P_y \\), this can be done by subtracting the base geometry (often squares). We do this again when we are taking the moment.

The tool below shows how the x and y components of the pressure differ when the depth of the curve is increase. Use the slider to change the depth of the curved plate, observe how the pressure force change. The <span style="color: #18a558; font-weight: bold;">green arrow</span> represents the local pressure distribution, the <span style="color: #2818d6; font-weight: bold;">red arrow</span> represents the vertical pressure force \\(F_{P,y}\\). and the <span style="color: #d61818; font-weight: bold;">red arrow</span> represents horizontal pressure force \\(F_{P,x}\\).

<!-- Source Code: [Google Colab](https://colab.research.google.com/drive/1sVnTfULUzD7w4L5td5ddyk8MWACJa9HN?usp=sharing) -->

{{< curved-plate-pressure >}}