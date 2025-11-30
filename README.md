# Dye-Indicator-Model
This repository supports a University of Washington project to develop a low-cost imaging tool that measures pH changes induced by coatings that host dye indicators.  The first milestone of this project is to use pH indicator strips as reliable quantitative sensors, achieving properties established by UNICEF. Ultimately, we plan to use these tools to screen for hypoxic-ischemic encephalopathy in babies.

Acid–base dye indicators exist as two pH-dependent conjugated forms, and their observed spectra can be modeled as a continuum between these forms — effectively a mixture of two dyes. The figure below shows the conjugated structures for bromothymol blue.
<br><br>
<p align="center" width="100%">
    <img width="60%" src="https://github.com/timrobinson/Dye-Indicator-Model/blob/main/structure.png"> 
</p>
<br>
The model is then:
<br><br>
<p align="center">
  <img src="https://latex.codecogs.com/svg.latex?\normalsize%20A_{\mathrm{meas}}(\lambda)=A_{\mathrm{H^+}}(\lambda)+A_{\mathrm{OH^-}}(\lambda)" alt="Absorption Equation"/>
</p>
<br>
The critical attributes, specifically the spectra at the conjugated extremes and the pH-dependent peak absorption of each conjugated form, can be obtained or digitized from open-sourced lit (the digitized attributes for bromothymol blue are provided as .csv in this repository).  Once obtained or digitized, the attributes can be plotted as shown below:
<br><br><br>
<p align="center" width="100%">
    <img width="90%" src="https://github.com/timrobinson/Dye-Indicator-Model/blob/main/dye_attributes.png"> 
</p>
<br>
where the dashed vertical lines on the right graph bound the physiological pH range.
