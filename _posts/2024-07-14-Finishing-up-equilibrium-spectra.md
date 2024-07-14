---
layout: post
title: Finishing up equilibrium spectra
categories: [GSoC]
---
- Tests have been added for the implementation of the Kurucz database and associated parts of the code
- Examples have been added relating to the Lorentzian broadening of atomic lines and partition functions.
- The function to parse Kurucz linelists has been re-written based on Pandas.
- The precision of some parts of the code has been improved by using `numpy.expm1` rather than `numpy.exp`, thereby showing weaker spectra that otherwise weren't being seen
- Support has been added for loading existing databanks of atomic species without specifying the species initially.
- A greater range of formats are now accepted as input to specify the species for which to calculate a spectrum.
- Documentation for atomic spectra and the Kurucz database has been updated further