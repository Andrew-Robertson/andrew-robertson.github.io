---
title: "Emulator-Assisted Calibration of a Semi-Analytic Galaxy Formation Model for the Roman Galaxy Redshift Survey"
authors:
  - admin
  - Andrew Benson
date: "2026-09-09T00:00:00Z"

publication_types: ["article"]
publication: "arXiv"

abstract: |
  Mock catalogues for the Roman Galaxy Redshift Survey benefit from galaxy populations whose physical properties and emission-line observables are predicted within a single galaxy-formation framework. We present an emulator-assisted calibration of the semi-analytic model Galacticus for this purpose. Because direct posterior exploration with Galacticus is computationally prohibitive, we train Gaussian-process emulators to predict the observables entering the calibration likelihood.

  We calibrate the model simultaneously to stellar mass functions, the star-formation-rate function, size--mass relations, the black-hole mass--velocity-dispersion relation, the mass--metallicity relation, and H-alpha luminosity functions. Combining these observables breaks parameter degeneracies present in individual fits and can reveal tensions where different observables favour different regions of parameter space.

  The resulting model provides a broadly successful simultaneous description of the calibration data, including the abundance and redshift evolution of H-alpha emitters relevant to the Roman Galaxy Redshift Survey. A direct Galacticus calculation at the maximum a posteriori point gives similarly good agreement with the calibration data, providing a calibrated galaxy-formation model suitable for constructing physically consistent mock catalogues for Roman.

summary: "Using emulators to calibrate Galacticus against multiple observations, producing a galaxy formation model for Roman mock catalogues."

tags:
  - Galaxy formation
  - Galacticus
  - Roman

featured: true

links:
  - type: custom
    label: Paper
    url: https://ui.adsabs.harvard.edu/abs/2026arXiv260910680R/abstract
  - type: custom
    label: arXiv
    url: https://arxiv.org/abs/2609.10680

image:
  preview_only: false
---

To prepare for the Roman Space Telescope's galaxy redshift survey, we need realistic simulated galaxy catalogues. Creating these requires models that reproduce several observed properties of galaxies at the same time.

In this work, we use fast statistical emulators to explore the parameters of the [Galacticus](https://github.com/galacticusorg/galacticus/wiki) galaxy formation model. These emulators approximate the model's predictions, making it practical to calibrate the model against a broad range of observations, including galaxy masses, sizes, and emission line luminosities.

Fitting these observations together helps constrain parameters that individual measurements cannot pin down on their own. It also reveals where different observations favour different model settings. We check the resulting calibration with a direct Galacticus calculation and find similarly good agreement with the data.

We have used the calibrated model to create simulated galaxy catalogues, which are now being used to generate pixel-level mock observations of Roman’s spectroscopic survey. These mock data are already helping to test the Roman spectroscopic analysis pipeline. They will be publicly released before Roman’s first science data release, allowing researchers to test their own analysis pipelines in advance.
The tools developed for this work are available in the <a href="https://github.com/Andrew-Robertson/Galacticus-emulation">GalacticEmu repository</a>. You can also explore how changing the model parameters affects its predictions using the <a href="https://galacticus-emulation.onrender.com">interactive emulator demo</a> (it takes a minute to fire up!).



