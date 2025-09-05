# Canadian Social Determinants Urban Laboratory (CSDUL)

## Overview

The **Canadian Social Determinants Urban Laboratory (CSDUL)** is a research infrastructure designed to advance the study of social determinants of health in Canada using linked data. It integrates information from over 15 major data sources, anchored by the **Canadian Population Health Survey (CPHS)**, to support multi-level statistical analyses of social and non-social factors affecting health outcomes. More details about CSDUL is located in the document: [**CSDUL Framework: Architecture, Processes, and Standards**](https://drive.google.com/drive/folders/1P0YVkB8RRvYBs-R5tm-pvqsE8GZDfYZb)
  

CSDUL is structured around a central **Hub** and five **Nodes**:

| Node | Focus Area |
|------|------------|
| Hub | [Individual Health](https://github.com/csdul/pre_beta_hub_individual)  |
| Node 1 | [Political Economic Context](https://github.com/csdul/pre_beta_political_economics_context) |
| Node 2 | [Environmental Context](https://github.com/csdul/pre_beta_environmental_context) |
| Node 3 | [Socioeconomic Context](https://github.com/csdul/pre_beta_socioeconomic_context) |
| Node 4 | [Material Circumstances](https://github.com/csdul/pre_beta_material_circumstances) |
| Node 5 | [Health System](https://github.com/csdul/pre_beta_health_system) |

Each Node is led by an investigator and collaborates with the Hub to generate, validate, and integrate indicators. Data is primarily housed in **Statistics Canada’s Research Data Centers (RDC)**, with selected outputs maintained in **CSDUL-OUT** on GitHub.  

## CSDUL Framework
![image](https://github.com/csdul/images/blob/main/csdul%20overview.png)

---
**Structure, Processes, and Standards**

CSDUL is structured around six core components that define its organization, clarify roles, and establish processes and standards:

1. Folders and files’ structure  
2. Process workflow  
3. Work communication standards  
4. Data structure standards  
5. Coding standards  
6. Documenting social determinants in CSDUL  

For more details about pount 3-6, please visit: [**CSDUL Framework: Architecture, Processes, and Standards**](https://drive.google.com/drive/folders/1P0YVkB8RRvYBs-R5tm-pvqsE8GZDfYZb)

## 1. CSDUL Folder and Files Structure

CSDUL ensures each indicator is well-documented, transparent, and reproducible. For every indicator, the following must be included:

- Tables of indicators derived from data sources  
- Code used to generate the indicator  
- Technical documentation describing construction and sources  
- End-user documentation (e.g., codebooks)  
- Published studies or validation materials supporting robustness  

CSDUL is maintained in two main environments:

- **CSDUL-OUT**: GitHub repositories  
- **CSDUL-RDC**: Statistics Canada Research Data Centres  

Both environments share the same folder structure, organized into Nodes and Hub. 

Each Node and Hub folder contains indicator subfolders, each organized into four standard folders:

1. **Codes** – scripts and programming files for data processing and outputs  
2. **Data** – raw or processed datasets for indicator development  
3. **Documents** – metadata, technical notes, and methodological explanations  
4. **Results** – summary tables, visualizations, and indicator values  

This structure ensures **consistency, collaboration, and long-term replicability** of CSDUL outputs.

---
## 2. Process Workflow

The general workflow for incorporating indicators into CSDUL is summarized in **Figure 1** and consists of four stages:

- **Generate**: Nodes generate social health indicators.  
- **Validate**: The Hub verifies inputs for accuracy. Issues are flagged and corrected early.  
- **Load**: Inputs are loaded into CSDUL by the Hub.  
- **Integrate**: Components are integrated to generate new health indicators and analyses.  

### Figure 1: General CSDUL workflow 
![image](https://github.com/csdul/images/blob/main/csdul%20general%20workflow.png)

## Detailed Workflow: Hub and Nodes Interaction

The detailed process for integrating new indicators into CSDUL is shown in **Figure 2**.  

#### CSDUL-RDC Process
1. **Start**: Nodes generate or review inputs and complete forms.  
2. **Share inputs with Hub**: Nodes send inputs to the Hub.  
3. **Validation**: Hub checks forms and files.  
   - **If No**: Returned to nodes for correction.  
   - **If Yes**: Hub saves files into CSDUL-RDC.  
4. **Release**: Hub releases the saved files.  
5. **Storage**: Released files are saved in CSDUL-OUT.  
6. **End**: Process complete.  

#### CSDUL-OUT Process
1. **Start**: Nodes generate or review files and complete forms.  
2. **Share with Hub**: Nodes send files to the Hub.  
3. **Validation**: Hub checks forms and files.  
   - **If No**: Returned to nodes for correction.  
   - **If Yes**: Hub saves files into CSDUL-OUT.  
4. **Import**: Hub imports files into RDC.  
5. **Storage**: Imported files are saved into CSDUL-RDC.  
6. **End**: Process complete.  

### Summary
- **CSDUL-RDC**: Nodes → Hub validation → RDC save → OUT.  
- **CSDUL-OUT**: Nodes → Hub validation → OUT save → RDC.  

### Figure 2: Detailed workflow to add inputs to CSDUL-RDC and CSDUL-OUT
![image](https://github.com/csdul/images/blob/main/csdul%20process%20to%20add%20inputs.png)

---

## If you have any questions or requests, please feel free to contact the CSDUL team:

- **Contact Email**: [daniel.yc@usask.ca](mailto:daniel.yc@usask.ca)
- **CSDUL Website**: [https://uphn.ca/CSDUL](https://uphn.ca/CSDUL)
