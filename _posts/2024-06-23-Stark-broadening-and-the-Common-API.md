---
layout: post
title: Stark broadening and the Common API
categories: [GSoC]
---
Stark broadening for atomic lines has been implemented with different temperature scalings for neutral and ionised radiators.

I integrated the API for atomic Kurucz linelists into the Common API, and in doing so the issue related to `truncation` and `optimization` seems to have been resolved.

The main differentiating aspect so far in the Common API for Kurucz is that new versions of linelists and lab lines aren't available for all species, the result being that the url from which to download the Kurucz linelist isn't known with certainty before actually attempting to download it, so the possibilities are ranked and attempted in order of preference and the first to return a valid response is used.