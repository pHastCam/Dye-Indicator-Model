This repository supports a University of Washington project to develop a low-cost imaging tool that measures pH changes induced by coatings that host dye indicators.  The first milestone of this project is to use pH indicator strips as reliable quantitative sensors, achieving properties established by UNICEF. Ultimately, we plan to use these tools to screen for hypoxic-ischemic encephalopathy in babies.


## Dye-Indicator-Model
This repository supports a University of Washington project to develop a low-cost imaging tool that measures pH changes induced by coatings that host dye indicators.  The first milestone of this project is to use pH indicator strips as reliable quantitative sensors, achieving properties established by UNICEF. Ultimately, we plan to use these tools to screen for hypoxic-ischemic encephalopathy in babies.

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

## Repository Guide

### 🔧 Installation Guide

Follow these steps to set up the environment and run the code:

1. **Create a working folder** on your local machine and move into it:

> mkdir Projects

> cd Projects

2. **Obtain the repository**

> git clone https://github.com/timrobinson/Dye-Indicator-Model.git

> cd Dye-Indicator-Model

3. **Create the conda environment**

> conda env create -f environment.yml

4. **Activate the environment**

> conda activate dye-indicator-model

 **Note on names:**  
 - The repository folder name (`Dye-Indicator-Model`) is created when you clone or unzip the project.  
 - The conda environment name (`dye-indicator-model`) comes from the `environment.yml` file.  
 - These names are independent: use the folder name when navigating with `cd`, and use the environment name when activating with `conda activate`.

## 📦 Dependencies

This project uses a conda environment defined in `environment.yml`.  
Key dependencies include:

- **Python** (version specified in `environment.yml`)
- **NumPy** – numerical computing
- **Pandas** – data manipulation and analysis
- **Matplotlib** – plotting and visualization
- **SciPy** – scientific computing
- **Jupyter** – interactive notebooks

## ▶️ Usage

Once the environment is active and you are inside the repository folder (`Dye-Indicator-Model`):

**Launch Jupyter Notebook** (requires Jupyter installed):

> jupyter notebook
  
- Navigate to the notebook file (e.g., filename.ipynb) in the browser interface.
- Open and run cells interactively.


