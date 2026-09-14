---
title: "Starting My PostDoc at the ATOMS Lab! 🌀"
layout: "simple"
summary: "Joining Prof. Cristina Amon's ATOMS Laboratory as a PostDoc to build deep-learning surrogate models for wind farm turbine placement."
categories: ["Announcements", "Academia", "Research"]
tags: ["PostDoc", "Machine Learning", "CFD", "Wind Energy", "UofT", "Autoencoder"]
date: 2026-09-10
draft: false
gallery_media:
  - src: "/img/posts/postdoc-geometry-mesh.png"
  - src: "/img/posts/postdoc-pipeline.png"
---

<div style="text-align: center;">

{{< gallery-slider >}}

</div>

<div style="text-align: justify;">

I'm excited to share that I've started my PostDoc at the **[ATOMS Laboratory](https://atoms.mie.utoronto.ca/energy-systems/)**, working with **Prof. Cristina Amon** in the Department of Mechanical & Industrial Engineering at the University of Toronto, continuing the lab's ongoing work on wind energy systems. My project focuses on **wind farm turbine placement with deep autoencoders**. The goal is to build a surrogate model that can learn the relationship between wind turbines layout and their resulting flow field, to enable rapid evaluation of wind turbine placement payouts.

To optimize gernealization, I am generating a training database of ~10,000 3D RANS simulations, each with 25 randomized wind turbines placement sampled using **Latin Hypercube / orthogonal sampling**. The case setup is fully auomated with 'Python', `snappyHexMesh`, and solved with the `SIMPLEC` algorithm on the Trillium CPU cluster, then sampled with VTK and being fed into a **deep 3D convolutional autoencoder** (trained on Trillium GPU nodes) to predict the velocity, pressure, turbulence fields, and drag coefficients  from the turbine layout geometry. Once trained, this surrogate model is intended to serve two purposes: giving CFD engineers a **near-instant preliminary prediction** for a proposed layout, and eventually acting as the fast reward-evaluation step inside a **reinforcement learning loop** to optimize turbine placement across different terrains.


</div>
