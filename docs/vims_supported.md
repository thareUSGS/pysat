---
layout: docs
title: Cassini Vims 
prev_section: mi_supported
next_section: requestformat
permalink: /docs/vims_supported/
---

PySAT supports level 1 Cassini VIMs in ISIS3 <code>.cub</code> format.  This is an initial reader that requires that the [ISIS3](http://isis.astrogeology.usgs.gov/Application/presentation/Tabbed/vims2isis/vims2isis.html) program <code>vims2isis</code> be used to convert from raw BIL format into an ISIS3 format that PySAT parses.

![Vims example](../../img/vims_supported/vims.png)

The PySAT VIMs reader renders just like the other data source specific readers enabling point and area spectra extraction.
