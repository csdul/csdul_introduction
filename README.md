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

Each Node is led by an investigator and collaborates with the Hub to generate, validate, and integrate indicators. Data is primarily housed in **Statistics Canada’s Research Data Centers (RDC)**, with selected outputs maintained in **CSDUL-OUT** on GitHub. The document that must be completed for each indicator added to CSDUL should include all the information outlined in the following template: [Document - add inputs to CSDUL] (https://github.com/csdul/csdul_introduction/blob/main/documents/add_inputs_to_csdul.md)  

## Datasets

The **CSDUL** works with a variety of administrative and public datasets. These datasets are processed, merged, and used to generate indicators for descriptive and statistical analyses. The datasets used are as follows:


- [Census](https://www12.statcan.gc.ca/census-recensement/index-eng.cfm)  
- [Correspondence File](https://www12.statcan.gc.ca/census-recensement/2021/geo/aip-pia/correspondence-correspondance/index-eng.cfm)  
- [Canadian Vital Statistics - Death Database (CVSD)](https://www23.statcan.gc.ca/imdb/p2SV.pl?Function=getSurvey&SDDS=3233)  
- [National Household Survey (NHS)](https://www23.statcan.gc.ca/imdb/p2SV.pl?Function=getSurvey&SDDS=5178)  
- [Discharge Abstract Database (DAD)](https://www.statcan.gc.ca/en/microdata/data-centres/data/cencchs-dad)  
- [National Ambulatory Care Reporting System (NACRS)](https://www.statcan.gc.ca/en/microdata/data-centres/data/dad-nacrs-omhrs-cvsdd)  
- [Canadian Census Health and Environment Cohorts (CanCHEC)](https://www.statcan.gc.ca/en/microdata/data-centres/data/canchec)  
- [Canadian Classification of the Functions of Government (CCOFOG)](https://www.statcan.gc.ca/en/statistical-programs/document/5218_D3_V3)  
- [Canadian Social Environment Typology (CanSET)](https://www150.statcan.gc.ca/n1/en/catalogue/17200002)  
- [Canadian Population Health Survey (CPHS)](https://www.statcan.gc.ca/en/microdata/data-centres/data/cchs)  
- [Longitudinal Administrative Databank (LAD)](https://www.statcan.gc.ca/imdb-bmdi/4107-eng.htm)  
- [Postal Code Conversion File Plus (PCCF+)](https://www150.statcan.gc.ca/n1/en/catalogue/82F0086X)  
- [Material and Social Deprivation Index (Pampalon Index)](https://www.inspq.qc.ca/en/deprivation/material-and-social-deprivation-index)  
- [Canadian Index of Multiple Deprivation (CIMD)](https://www23.statcan.gc.ca/imdb/p2SV.pl?Function=getSurvey&SDDS=5274)  
- [DMTI Spatial’s CanMap Enhanced Points of Interest (EPOI)](https://www.dmtispatial.com/)  
- [Supply and Use Tables](https://www150.statcan.gc.ca/n1/pub/15-602-x/15-602-x2017001-eng.htm)  
- [Input-Output Economic Multipliers](https://open.canada.ca/data/en/dataset/8e56cad4-4e1b-4e7d-be21-5034feb6190a)  
- [Canadian Urban Environmental Health Research Consortium (CANUE)](https://canue.ca/)

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

For more details about points 3-6, please visit: [**CSDUL Framework: Architecture, Processes, and Standards**](https://drive.google.com/drive/folders/1P0YVkB8RRvYBs-R5tm-pvqsE8GZDfYZb). Points 1 and 2 are briefly presented below. 

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
