---
layout: docs
title: Spectral Calculator
prev_section: mgm
next_section: troubleshooting
permalink: /docs/calc/
---

<div class="note warning">
  <h5>Proof of Concept</h5>
  <p>This functionality is not fully implemented!  Things will break or not work as expected.</p>
</div>

We understand that both spectral and band math are essential features of an exploratory workflow.  Additionally, we are seeking to support an integrated work environment where moving ASCII spectra to another environment (R, Excel) is not required.

The Spectral Calculator is a proof of concept highlighting the potential to extend PySAT functionality.

## Spectral Calculator
To open calculator select it from the tool menu.

![Spectral Calculator](../../img/calc/open.png)

<div class="note">
  <h5>Empty Spectral List</h5>
  <p>The calculator does not automatically reload when additional spectra are visualized.  To refresh the spectra list, simple click the refresh button (directly above the list).</p>
</div>

![Calc](../../img/calc/calc.png)

The calculator supports basic mathematical functions on image spectra.  To add a spectra to the equation bar, simple double click the name in the spectra list.

![Equation](../../img/calc/equation.png)

A dropdown menu below the calculator allows selection of a destination for the computed spectra.  This can be a new plot or one of the currently open plots.

<div class="note">
  <h5>Offset</h5>
  <p>Adding a derived spectra to an existing plot utilizes the offset spinbox.  If you are comparing spectra and wish them to stack without artificial offset, be sure to set the offset to 0.</p>
</div>


Below are the results of averaging two spectra - a basic proof of concept example.  The plot title is the equation used to derived the spectra.

![Results](../../img/calc/results.png)


