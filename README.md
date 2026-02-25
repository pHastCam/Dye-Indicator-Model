# Project pHastCam: Bromothymol Blue Dye Indicator Modeling

Acid–base dye indicators exist as two pH-dependent conjugated forms, and their observed spectra can be modeled as a continuum between these forms — effectively a mixture of two dyes. The figure below shows the conjugated structures for bromothymol blue.
<br><br>
<p align="center" width="100%">
    <img width="60%" src="https://github.com/timrobinson/Dye-Indicator-Model/blob/main/structure.png"> 
</p>
<br>
The absorption spectral model is then:
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
where the dashed vertical lines on the right graph bound the physiological pH range. By applying the digitized data described above to the repository associated .ipynb file, the following plot can be obtained:
<br><br><br>
<p align="center" width="100%">
    <img width="50%" src="https://github.com/timrobinson/Dye-Indicator-Model/blob/main/demo.png"> 
</p>
<br>
where the bold lines represent the spectra within the physiological pH range.  These spectra represent a single component in the model of the imaging system used to quantify pH.

## Installation    
1. Clone the repository
    git clone https://github.com/pHastCam/Dye-Indicator-Model.git
    cd Dye-Indicator-Model
2. Create the conda environment from YAML file
    conda env create -f environment.yml
3. Activate the environment
    conda activate Dye-Indicator-Model
4. Launch Jupyter Notebook

## Usage
1. When the environment is active, launch Jupyter Notebook 
2. Open to the notebook associated with the code in the browser interface
3. Note that this code uses data files that in the CSV format, users must make sure that the files called match the appropriate name on their computer and are in the correct location.

## Built with
Python=3.9.13
Numpy=1.21.5
Scipy=1.9.1
Pandas=1.4.4
Matplotlib=3.5.2




