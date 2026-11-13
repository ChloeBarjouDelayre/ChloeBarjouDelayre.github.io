---
layout: page
title: H₀ anisotropy
---

The cosmological principle assumes the isotropy of the Universe at large scales. Recent disagreements with the standard model motivate the investigation of possible anisotropies in the Universe. A possible anisotropy could be observed in the Hubble constant: H₀. My research work focused on creating a method to measure this anisotropy in the Zwicky Transient Facility (ZTF) type Ia Supernovae (SN Ia) sample. The large footprint and efficient sampling of ZTF allow for a H₀ anisotropy measurement with unprecedented precision. I started by focusing on the simplest version of a multipole which can reproduce anisotropy, a dipole. A dipole is a preferred axis; a figure representing a dipole with an amplitude of 3 km/s/Mpc is shown below. In this figure, the effect of this preferred axis is depicted across the entire sky. The goal was to develop an original method capable of fitting a dipole to the data. To develop this, I used realistic ZTF simulations and introduced a known dipole (with an amplitude of 3 km/s/Mpc) into these simulations in order to construct a likelihood function that would allow us to recover this initial dipole. To achieve this, 27 independent simulations were used, and 48 different dipole positions were tested. 

<figure>
  <img src="{{ site.baseurl }}/assets/Inital_dipole.png" alt="Introduced dipole" style="width: 70%;">
  <figcaption>Skymap colored following the amplitude of the dipole in red stars representing the initial dipole direction (α0 = 90.0°, δ0 = 19.47°) of an amplitude of 3 km/s/Mpc.</figcaption>
</figure>

Several systematic approaches were studied, they are all summarized in the figures below. Among them, the use of different dustmaps made it possible to observe their impact on the measurement. Two different dust maps were used: the Planck2013 map and the SFDMaps. The results of using an older, and therefore less accurate, map are shown in the figure above; we can see that, on average, it is more difficult to recover the initial amplitude in this case. Another of the key systematics I tested was sky coverage, I tested it by producing different versions of the ZTF simulations. In particular, I tested the impact of removing the southern sky or the Milky Way and the impact of the ZTF cadence. This analysis suggests that the method is not affected by the sky coverage while the cadence of observations introduces a small bias as a function of the dipole direction.

<figure>
  <img src="{{ site.baseurl }}/assets/diffsyst.png" alt="Systematic effects on dipole parameters">
  <figcaption>Comparison of systematic effects on the dipole amplitude (km/s/Mpc), right ascension (°) and declination (°). The vertical black line is the zero reference.</figcaption>
</figure>

 All of these systematic studies have made it possible to develop an error model that accounts for both statistical and systematic errors. This allows us to assums that the injected dipole is recovered without bias, whatever H₀ is assumed. For example, for an initial dipole with an amplitude of 3 km/s/Mpc, we find this dipole with the following error: 

<div style="display:flex; flex-wrap:wrap; border-top:1px solid rgba(128,128,128,.4); border-bottom:1px solid rgba(128,128,128,.4); margin:1.5rem 0 0.5rem;">
<div style="flex:1 1 220px; padding:1rem 1rem 1rem 0;">
<div style="font-size:2.6rem; line-height:1.1;">0.33 <span style="font-size:0.9rem; color:#6fbf8e;">km s⁻¹ Mpc⁻¹</span></div>
<div style="opacity:.7; font-size:0.9rem;">error on the H₀ dipole amplitude</div>
</div>
<div style="flex:1 1 160px; padding:1rem; border-left:1px solid rgba(128,128,128,.4);">
<div style="font-size:2.6rem; line-height:1.1;">3.4°</div>
<div style="opacity:.7; font-size:0.9rem;">error on its right ascension</div>
</div>
<div style="flex:1 1 160px; padding:1rem; border-left:1px solid rgba(128,128,128,.4);">
<div style="font-size:2.6rem; line-height:1.1;">6.1°</div>
<div style="opacity:.7; font-size:0.9rem;">error on its declination</div>
</div>
</div>
<p style="font-size:0.9rem; opacity:.8;">Recovery of a 3 km s⁻¹ Mpc⁻¹ dipole injected into realistic simulations of the ZTF DR2 supernova sample. <a href="https://arxiv.org/abs/2601.11139">arXiv:2601.11139</a></p>



