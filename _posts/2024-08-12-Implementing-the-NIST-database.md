---
layout: post
title: Implementing the NIST database
categories: [GSoC]
---
- The Einstein A coefficient is now used directly for calculating the non-equilibrium linestrength, given that it is calculated anyway for non-equilibrium spectra where it isn't already present, rather than removing the temperature-dependent component of the reference linestrength, which was found to result in some atomic spectra not appearing. This also removes the need to calculate the reference linestrength for databanks where it's not already present.
- Removed some redundnant code and miscellaneous fixes and improvements.
- Fixed the documentation for many parts of the new code for atomic spectra so the formatting appears correct on Read the Docs.
- The pull request for the implementation of the Kurucz database has been merged
- Work has started on adding support for the NIST atomic database and it is currently at a stage where it produces working spectra.