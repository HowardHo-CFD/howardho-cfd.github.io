---
title: "Cone Viscometer 🔽"
layout: "simple"
showDate: false
showReadingTime: false
showWordCount: false
build:
  list: never
---

{{< katex >}}

<div class="project-img">
<video src="/img/teaching/cone-viscometer-velocity.mp4" class=" rounded-lg" autoplay loop muted playsinline onclick="openMediaLightbox(this)"></video>
</div>

The video above shows how the velocity profile varies when the altitude h and radius r changes. The height of the cone viscometer is exagerrated to show the linear velocity profiles (real cone viscometers has an average angle of about \\(1^o\\) ). The video below segments the surface into 4 parts with equal height, we can see that as we move upward, the shear force increases, eventhough \\(\tau\\) remained constant, this is due to the increased local surface area. This has a direction impact on the way Torque is calculated, near the bottom, both radius and local shear force are small comapred to the top, therefore, integration is needed to calculate the torque.

<div class="project-img">
<video src="/img/teaching/cone-viscometer-shear-force.mp4" class=" rounded-lg" autoplay loop muted playsinline onclick="openMediaLightbox(this)"></video>
</div>


For the interactive tools below, use the slider to change the line plot altitude \\(h\\) and radius \\(r\\), observe how the velocity profile \\(v_\theta\\) change. <i><span style="font-weight;"><span style="color: #ef4444;">Note that for the 2nd plot, \\(v_\theta\\) was rotated for visualization (technically it should be into/out of the page).
</span>

<!-- Source Code: [Google Colab](https://colab.research.google.com/drive/1OOirNwnnebM2w55GMmz79ogSlh9vie_a#scrollTo=NtCxuEuoCP6Z) -->

{{< cone-viscometer >}}

<!-- {{< cone-viscometer-iso >}} -->