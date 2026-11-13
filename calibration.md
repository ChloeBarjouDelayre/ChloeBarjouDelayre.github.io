---
layout: page
title: Filter Calibration
---

For precision cosmology, accurate photometry of the observations is required. Consequently, I worked on creating a realistic model for the ZTF filter. This model, called synthetic filters, takes into account all the optics of the ZTF telescope, the real angle of incidence of the light, and the difference between the two types of CCD in ZTF (single coating and double coating) show in the figure below.

<figure>
  <img src="{{ site.baseurl }}/assets/optics_cam_telescop.jpeg" alt="Systematic effects on dipole parameters">
  <figcaption>The left panel show cutaway view of the Samuel Oschin Telescope highlighting ZTF subsystem with a transmission mesurement. Illustration from Dekany et al. The right panel contains an illustration of the camera with the different layer of CCD. </figcaption>
</figure>

In order to create a model that is as realistic as possible, I verified the quality of the synthetic filters by calibrating them with Gaia star spectra, comparing the magnitudes of observed stars from ZTF ($$m_{\text{ZTF}}$$) by integrating Gaia spectra over the synthetic filters ($$m_{\text{Gaia}}$$). his comparison is performed using the following equation: $$m_{\text{ZTF}}+ZP-m_{\text{Gaia}}$$ where we have to fit $$ZP$$, which is the zero point (this zero point is a correction that compensates for unaccounted-for effects, thereby harmonizing the data), per Modified Julian Date (MJD) and quadrants. By comparing this difference in magnitude with the colors of the reference stars, we observed a non-zero difference in magnitude. Which imply that the synthetic filters are not as realistic as needed, a more precise measurement on the instrument was necessary. To adjust the synthetic filters, we need more measurements of the real filters. To do this, I joined the Travel Collimated Beam Projector (TCBP) experiment. The TCBP is the traveling version of the CBP [6], a standard, adjustable beam light for telescope calibration. I contributed to a
three week calibration campaign at the Palomar Observatory to measure the transmission of the optics of the ZTF telescope and the CCD quantum efficiency with and without filters. During the campaign I was responsible for quantifying the intensity and location of a ghost (light reflections in the CCD) in each image to avoid contamination.
