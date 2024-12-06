# Introduction to CSDUL

This repository contains the key documents that govern the operation of CSDUL. These documents explain various processes associated with the project. They include:

- **[Coding Standards](https://docs.google.com/document/d/17h79bGMTlEYICTR_gD_mV9XaFS2JQmzFCMC_w5CI0kc/edit?tab=t.0)**: Guidelines and protocols for coding within the project. It defines rules for naming conventions, formatting, and structuring code to ensure consistency and accuracy across the system.
  
- **[Process to Add Inputs into CSDUL](https://docs.google.com/document/d/1ig7-2o3SWa7oVhyf-YDoMvn5qlT0VHx-eUM-Dx_XFaQ/edit?tab=t.0)**: This document outlines how new data or inputs are incorporated into the CSDUL system. It includes steps for validation, formatting, and quality assurance to maintain the integrity of the dataset.

- **[Organization Chart](https://drive.google.com/file/d/1Ua1ioOLbiCRUBbGCvqOc84TH2xNAs38l/view?usp=drive_link)**

- **Workflow**: Diagrams that illustrate the structure and operational flow of the CSDUL system, showing how different components interact and the steps involved in the data processing pipeline.

- **Hub and Nodes**: Hub and Nodes role and components set up. There is one Hub and five Nodes:
  - **Hub**   : [Individual Health](https://github.com/csdul/pre_beta_hub_individual) 
  - **Node 1**: [Political Economic Context](https://github.com/csdul/pre_beta_political_economics_context)
  - **Node 2**: [Environmental Context](https://github.com/csdul/pre_beta_hub_individual_health)
  - **Node 3**: [Socioeconomic Context](https://github.com/csdul/pre_beta_socioeconomic_context)    
  - **Node 4**: [Material Circumstances](https://github.com/csdul/pre_beta_material_circumstances)
  - **Node 5**: [Health System](https://github.com/csdul/pre_beta_health_system)

## CSDUL **Workflow**
![image](https://github.com/user-attachments/assets/b4c8a4ba-49db-4e8e-b4bb-f189e0de3b5a)

## Definitions

### Data Sources
These are the various sources of information used in the CSDUL system.

### Generate
Nodes generate social health indicators based on the input data.

### Validate
The Hub verifies inputs to ensure their correctness. Any issues identified are flagged and corrected at an early stage to maintain data integrity.

### CSDUL – Load
The Hub loads the validated inputs into CSDUL.

### CSDUL – Integrate
CSDUL components are integrated to generate new health indicators and analyses.

## Process to Incorporate Files Into CSDUL
![image](https://github.com/user-attachments/assets/1074f403-a706-4687-8097-e7027ddee57a)

## CSDUL Components Set Up by Hub and Nodes
![image](https://github.com/user-attachments/assets/ceee5ccc-7b18-4a40-9013-d898fc2c74e9)

## How Are CSDUL Indicators Organized?

Each indicator and model in the **CSDUL** is organized into the following folders:

- **Codes**: Contains scripts or algorithms used to calculate and process the indicator.
- **Documents**: Includes detailed documentation outlining the methodology, purpose, and any relevant notes for the indicator.
- **Tables or Datasets**: Contains the data used for calculating or representing the indicator.
- **Support Files** (if applicable): Provides additional resources such as configuration files, reference data, or supplementary models.

This repository is collaboratively developed by the **Nodes** and the **Hub**, ensuring an integrated approach to data management and indicator development.

## If you have any questions or requests, please feel free to contact the CSDUL team:

- **Contact Email**: [daniel.yc@usask.ca](mailto:daniel.yc@usask.ca)
- **CSDUL Website**: [https://uphn.ca/CSDUL](https://uphn.ca/CSDUL)
