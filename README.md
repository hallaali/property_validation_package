# property_validation_tool

## Contents of the GitHub: 
### Validation/Visualization Python Scripts (https://github.com/hallaali/property_validation_package/tree/main/validation_scripts)
#### Jet-A Fuel 
Within the "validation scripts directory (link above) there is a Python script called "Jet_A_validation_tool" (https://github.com/hallaali/property_validation_tool/blob/main/validation_scripts/jetA_validation_tool.py). This script contains the code used to generate the Jet-A fuel validation and visualization packages. 
#### Hydrogen 
The "validation_scripts" directory also contains a Python Script called "H2_validation_tool" (https://github.com/hallaali/property_validation_tool/blob/main/validation_scripts/H2_validation_tool.py). This script contains the code used to generate the Hydrogen visualization package. 
#### Template 
Lastly, the "validation_scripts" directory also contains a Python Script called "validation_tool_(template) (https://github.com/hallaali/property_validation_tool/blob/main/validation_scripts/validation_tool_(template).py). This script contains a general code for generating a validation/visualization package, where the lines enclosed in the symbol "!" indicate the fields that should be input by the user to complete the script for the selected fuel. 

### Data Files (https://github.com/hallaali/property_validation_tool/tree/main/data_files)
#### Jet-A Fuel
The jetA_data directory (https://github.com/hallaali/property_validation_tool/tree/main/data_files/jetA_data) contains the .csv files used to generate the validation/visualization packages for Jet-A fuel with the Jet-A validation Python script. All of the .csv files contained in this folder are called and read by Python in the validation script to plot the data directly from these files. 
#### Hydrogen
The hydrogen_data directory (https://github.com/hallaali/property_validation_tool/tree/main/data_files/hydrogen_data) contains the .csv files used to generate the visualization packages for Hydrogen with the Hydrogen validation Python script. All of the .csv files contained in this folder are called and read by Python in the validation script to plot the data directly from these files. 

### Validation/Visualization Packages (https://github.com/hallaali/property_validation_tool/tree/main/validation%2Bvisualization_packages)
#### Jet-A Fuel
The jetA_validation_package directory (https://github.com/hallaali/property_validation_tool/tree/main/validation%2Bvisualization_packages/jetA_validation%2Bvisualization_package) contains folders each named after the .csv data files that contain data for Jet-A fuel properties. Each of these folders contain validation/visualization plots from the corresponding .csv data file.
#### Hydrogen
Similarly, the H2_validation_package directory (https://github.com/hallaali/property_validation_tool/tree/main/validation%2Bvisualization_packages/H2_visualization_package) contains folders each named after the .csv data files that contain data for Hydrogen properties. Each of these folders contain visualization plots from the corresponding .csv data file.

## How to Use the Python-Based Property Validation Tool: 

### Using the Thermo Rig to Generate Data

### Generating the Python Validation Script for a Selected Fuel
In the "validation_scripts" folder there is a Python script that can be utilized as a template to be adjusted for a selected fuel (https://github.com/hallaali/property_validation_tool/blob/main/validation_scripts/validation_tool_(template).py). The areas enclosed in two "!" symbols vary with the selected fuel and should be filled in by the user. The H2 and Jet-A validation scripts can be used as examples. This section will outline all of the areas with "!" symbols and how they should be filled in:

**1.** *line 12* - **!filepath!**: Enter the filepath of the first .csv file with data for the selected fuel. This data file should be the "validation" portion (containing percent error between pkg and CEA values)

**2.** *line 24* - **!filepath!**: Enter the filepath of the second .csv file with data for the selected fuel. This data file should be the "visualization" portion (just the thermo properties, no percent error/calculation)

* More files can be added if necessary --> reuse the set of lines 12-18 (for validation) or lines 24-27 (for visualization) and create more dataframes (data3, data4, data5, etc.) *  

**3.** *line 49* - **!filepath!**: Enter the filepath of the folder that will contain the validation/visualization package folder

**4.** *line 59 and line 84*  - **!fuelname!**: Enter the name of the selected fuel (to be displayed on the plot titles)

**5.** *line 96* - 







### Running the Python Script from the Command Line
