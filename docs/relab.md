---
layout: docs
title: RELAB Spectral Library 
prev_section: clementine_derived
next_section: mgm
permalink: /docs/relab/
---

PySAT support visualization and processing of the [RELAB Spectral Database](http://www.planetary.brown.edu/relabdocs/relab_disclaimer.htm).  Users will need to [download](http://www.planetary.brown.edu/relabdata/) the RELAB database for use with PySAT.

To utilize RELAB, the user must fist identify the spectra of interest.  RELAB provides multiple <code>.xls</code> files to facilitate spectra location.  Take note of the spectra datafile location within the <code>data</code> directory.  This is the directory you will need to navigate to within PySAT

## Opening a RELAB Spectra
To open a relab spectra select <code>Open RELAB Spectra</code> within the <code>Spectral Libraries</code> from the main menu bar.  This opens a file dialog which prompt you to open the <code>.txt</code> or <code>.asc</code> that corresponds to the spectra of interest.

![RELAB](../../img/relab/open.png)

This loads the spectra into a new plot.

![RELAB](../../img/relab/plot.png)

To add this spectra to another plot, simply select the spectra, open the contextual menu, and select <code>Add Spectra To Plot</code>.

![RELAB](../../img/relab/context.png)

When the spectra in the plot and the RELAB spectra do not have the same node spacing (wavelength) we utilize a cubic spline to interpolate from the RELAB spectra to the extracted spectra.

![RELAB](../../img/relab/resample.png)

<div class="note warning">
  <h5>Compute Times</h5>
  <p>Cubic interpolation of spectra with many data points can be time consuming.  Please be aware if interpolating a RELAB spectra that is dense or covers many wavelengths.  A future enhancement may be to multithread the software so the GUI does not lock.</p>
</div>

Once resampling is complete, the spectra is added to the destination plot for further analysis.

<div class="note info">
  <h5>RELAB Spectra</h5>
  <p>In the destination plot, RELAB spectra are 'first class' objects.  They are treated identically to an extracted spectra and can be moved, smoothed, converted to point, etc.</p>
</div>




