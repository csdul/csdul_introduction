# Canadian Social Determinants Urban Laboratory

## Framework: Architecture, Processes, and Standards

**Prepared by Daniel Yupanqui**  
**August 2025**

---

## Table of Contents

1. [Purpose of this Document](#purpose-of-this-document)
2. [What is CSDUL?](#what-is-csdul)
3. [Structure, Processes, and Standards](#structure-processes-and-standards)
   - [1. CSDUL Folder and Files Structure](#1-csdul-folder-and-files-structure)
   - [2. Process Workflow](#2-process-workflow)
   - [3. Work Communication Standards](#3-work-communication-standards)
   - [4. Coding Standards](#4-coding-standards)
   - [5. Data Structure Standards](#5-data-structure-standards)
   - [6. Form to Add Social Determinants to CSDUL](#6-form-to-add-social-determinants-to-csdul)

---

# Purpose of this Document

This document aims to explain the structure of the **Canadian Social Determinants Urban Laboratory (CSDUL)** and establish the standards that guide collaboration between the Hub and the Nodes.

Its objective is to outline the organization of indicators and related documents in **CSDUL-OUT** and **CSDUL-RDC**, as well as to describe the process and work standards for incorporating new indicators or models into CSDUL.

---

# What is CSDUL?

This project aims to advance teaching and research on the use of linked data to improve the understanding of how the social determinants of health shape health outcomes in Canada.

CSDUL will consist of a suite of code and data components that integrate information from at least 15 major data sources. These components will generate variables to support multi-level statistical analyses of both social and non-social factors influencing health.

At the core of the project is the **Canadian Population Health Survey (CPHS)**, which links the country’s leading health survey—the **Canadian Community Health Survey (CCHS)**—with a wide range of administrative datasets.

Figure 1 provides a stylized overview of the CSDUL data structure and its organizing Nodes.

CSDUL will be structured around five **Nodes**, each led by an early- or mid-career investigator.

These Nodes will incorporate and validate indicators at macro, meso, and micro levels by leveraging leading sources of social and environmental data.

A central **Hub** will coordinate, assemble, and disseminate the outputs of CSDUL.

Importantly, CSDUL will be designed to operate on microdata housed within Statistics Canada’s **Research Data Centres (RDC)**.

### Figure 1. Overview of CSDUL

![Overview of CSDUL](images/csdul_overview.png)

---

# Structure, Processes, and Standards

CSDUL is structured and guided by six core components, which define its organization, clarify roles and responsibilities, and establish processes and standards:

1. Folders and files' structure
2. Process workflow
3. Work communication standards
4. Data structure standards
5. Coding standards
6. Document to add social determinants to CSDUL

---

# 1. CSDUL Folder and Files Structure

CSDUL is structured to ensure that each indicator is well-documented, transparent, and reproducible.

For every indicator, the following must be included:

- Tables of indicators derived from the data sources
- Code used to build the indicator
- Technical documentation describing how the indicators were constructed and which sources were used
- End-user documentation, such as codebooks, that explains the indicators and provides guidance on their use
- Published studies or validation materials that support and demonstrate the robustness of the work

To organize this information, CSDUL is maintained across two main environments:

- **CSDUL-OUT** — hosted in GitHub repositories
- **CSDUL-RDC** — located in Statistics Canada’s Research Data Centres

Both environments follow the same folder structure, organized into six main areas:

- **HUB – Individual Health**
- **Node 1 – Political Economic Context**
- **Node 2 – Environmental Context**
- **Node 3 – Socioeconomic Context**
- **Node 4 – Material Circumstances**
- **Node 5 – Health System**

Each Node folder contains a set of indicator subfolders.

Within each indicator subfolder, the required information is organized into four standard folders:

### 1. Codes

Scripts and programming files used to process data, generate indicators, and produce outputs.

### 2. Data

Raw or processed datasets forming the basis for indicator development.

### 3. Documents

Supporting materials such as metadata, technical notes, and methodological explanations.

### 4. Results

Outputs including summary tables, visualizations, and indicator values.

This structure ensures consistency across indicators, facilitates collaboration between the Hub and the Nodes, and supports the long-term replicability of CSDUL outputs.

---

## Current Status

As of **August 2025**, seven indicators have been added to CSDUL.

### HUB – Individual Health

- Avoidable Mortality
- Substance Use
- Population Counts
- CASDOHI
- Economic Multipliers by Sectors

### Node 1 – Political Economic Context

- CCOFOG and Macroeconomic Indicators

### Node 3 – Socioeconomic Context

- Family, Recreation, and Safety Resources

---

## Description of Folders

### Codes

Include scripts and programming files used to process data, generate indicators, and produce outputs.

### Data

Contains raw and processed datasets that serve as the basis for indicator development.

For indicators processed in RDC and subsequently added to CSDUL-OUT, the raw datasets cannot be included, as they are not available outside the RDC.

### Documents

Consist of supporting materials such as metadata, technical notes, and methodological explanations.

### Results

Store outputs from the codes and data, including summary tables, visualizations, and indicator values.

---

# 2. Process Workflow

The general workflow that describes the process of incorporating indicators into CSDUL is presented in Figure 2.

It is comprised of four stages:

1. **Generate**  
   Nodes generate social health indicators.

2. **Validate**  
   The Hub verifies the inputs to ensure they are correct. Any issues are flagged to the Node and fixed at an early stage.

3. **Load**  
   Inputs are loaded into CSDUL by the Hub.

4. **Integrate**  
   CSDUL components are integrated to generate new health indicators and analyses.

### Figure 2. General CSDUL Workflow

![General CSDUL Workflow](images/csdul_general_workflow.png)

---

## CSDUL-RDC Process

1. **Start**  
   The process begins when Nodes generate or review inputs and complete forms.

2. **Share inputs with Hub**  
   The Nodes then send these inputs to the Hub.

3. **Validation**  
   The Hub checks whether the forms and files are correct.

   - **If No:** The process returns to the Nodes so they can correct and resubmit the information.
   - **If Yes:** The Hub saves the files into CSDUL-RDC.

4. **Release**  
   After saving, the Hub releases the files.

5. **Storage**  
   The released files are then saved in CSDUL-OUT.

6. **End**  
   The process is complete.

---

## CSDUL-OUT Process

1. **Start**  
   The process begins when Nodes generate or review files and complete forms.

2. **Share with Hub**  
   The Nodes send the files to the Hub.

3. **Validation**  
   The Hub checks whether the forms and files are correct.

   - **If No:** The process returns to the Nodes for correction and resubmission.
   - **If Yes:** The Hub saves the files into CSDUL-OUT.

4. **Import**  
   After saving, the Hub imports the files into RDC.

5. **Storage**  
   The imported files are then saved into CSDUL-RDC.

6. **End**  
   The process is complete.

---

## In Simple Words

- **CSDUL-RDC** starts with Nodes creating inputs, validated by the Hub, saved in RDC, and then passed to OUT.
- **CSDUL-OUT** starts with Nodes creating files, validated by the Hub, saved in OUT, and then passed into RDC.

### Figure 3. Detailed Workflow to Add Inputs to CSDUL-RDC and CSDUL-OUT

![Detailed CSDUL Workflow](images/csdul_detailed_workflow.png)

---

# 3. Work Communication Standards

CSDUL is more than just a collection of indicators, codes, datasets, and models.

It represents a collaborative effort among a team of researchers who work together to create a richer data environment that supports both quantitative and qualitative research.

In this context, effective communication between each Node and the Hub is crucial for continuously adding valuable indicators and producing high-quality research.

To achieve this, three main work standards must be followed.

---

## Emails

Research assistants will generally produce indicators within Nodes. Similarly, in the Hub, the management of CSDUL will be handled by a research assistant or research specialist.

These researchers are responsible for coordinating the addition of new indicators, requesting information, or seeking technical support.

However, Node Leads and the Hub Lead must always remain informed of these communications to ensure proper oversight and timely decision-making.

The following email rules apply:

- All emails must copy both the **Node Leads** and **Hub Lead**, even if they are not directly involved in the discussion. This ensures awareness and readiness to intervene if necessary.
- Every email, whether between Nodes, from Nodes to the Hub, or from the Hub to Nodes, must be acknowledged and responded to within **3 business days**.

---

## Extraordinary Meetings

Nodes and the Hub are responsible for requesting meetings when clarifications, support, or problem-solving are needed.

The receiving party must make every reasonable effort to accommodate the meeting as soon as their schedule permits.

---

## Timeline for Corrections and Feedback

During the validation process, efficient communication between the Hub and the Nodes is critical to successfully integrating indicators into CSDUL with full supporting documentation.

The following timelines apply:

- When Nodes submit inputs to the Hub for inclusion, the Hub must **review, validate, approve, or request amendments within one week**. All feedback will be communicated via email.
- When the Hub requests corrections or amendments, Nodes must return the revised files **within one week** of receiving the request.
- If either the Hub or a Node cannot meet the one-week deadline, this must be promptly communicated to the other party. The message must explain the reason for the delay and provide a clear new deadline for submission.

---

## Data Requests

Building an indicator for inclusion in CSDUL may sometimes require sharing datasets or variables between Nodes, or between the Hub and Nodes.

These exchanges carry a high risk of miscommunication.

Working with datasets, especially when merges, collapses, or other data transformations are involved, is complex. Most errors tend to occur at this stage, and when the process involves geographically dispersed teams, the likelihood of problems with output increases significantly.

The data request should follow the steps below to minimize confusion and errors:

1. **Hold a meeting** between the Hub and the relevant Node(s) to discuss the data-sharing request.

2. **Clearly explain the data needed**, the purpose of requesting those variables, and provide a simple sketch of the desired table.

   This can be prepared in Excel, Word, Paint, or any other tool.

   The goal is to eliminate any ambiguity regarding the structure and content of the requested data.

3. **Send a written summary after the meeting by email.**

   This summary must explicitly state:

   - Agreements reached
   - Responsibilities assigned
   - Deadlines
   - A sketch of the requested table
   - Required variables

---

# 4. Coding Standards

## Purpose

This section proposes some basic coding rules to standardize coding work that will be included in CSDUL.

These rules are based on the **tidyverse style** and **Martin (2008)** and adapted for the type of work we do, which is scientific, and the context in which we work: the secure research environment of Statistics Canada’s Research Data Centres (RDC).

---

## Why is it Essential to Have Coding Rules?

Contrary to popular perception, the purpose of the code file (e.g., Stata Dofile or R Script) in scientific research is not to do data analysis—or at least not just that.

It is to create a written record of the work we have done to analyze our data so that it can communicate with others, including our **future selves**.

The computer analyzes our data; our work as researchers is to provide it with instructions, and it is this that needs to be documented.

To be clear for readers, these instructions should follow consistent rules that are used effectively.

Small details in our code can significantly impact the readability of our work and determine whether we are able to clearly understand and work with it to replicate, update, and make corrections if needed.

The written record of the work we are doing to analyze data is made up of a combination of the following:

1. Instructions to the computer to analyze our data.
2. Annotations that structure and explain these steps.

Since the ultimate purpose of your program is to communicate the work we are doing to analyze our data, it may help to think of our programs and documentation as **essays rather than merely as computer programs**.

---

## The Power of Clear Code in CSDUL

A clearly written program is a powerful thing.

It will be able to:

- Record the steps we have taken in any data analysis for others and ourselves to refer to.
- Allow CSDUL to provide programs and processes to researchers who have never touched the data before, while still enabling them to read the code and understand what it is doing.
- Allow anyone in the future to pick up CSDUL files and understand what they can do.
- Provide an easy way to modify or improve the analysis retrospectively.
- Help evaluate and debug the work. If something does not work as it should, the code file can be used to identify where mistakes have been made.
- Serve as an archive of all data analysis performed on a project.
- Provide a valuable repository of code that can be copied and adapted for future projects.
- Serve as a record of collaboration and as a principal mechanism through which collaborators communicate around a task.

On the other hand, if our code is not clearly written, does not communicate effectively, or is not easily readable, then the Hub and Nodes will have a hard time tracing the past steps taken in the project.

CSDUL will also be unable to effectively share its resources with researchers, and Nodes and the Hub may be unable to identify bugs in the code that need fixing.

The recommended rules are as follows.

---

## 4.1. Character Length

It is recommended that functions be as short as possible, with a maximum width of **80 characters**.

This recommendation also applies to comments inside the syntax.

Martin (2008) advises following **The Stepdown Rule**, which emphasizes that a program must be easily read from top to bottom rather than left to right.

Some software permits abbreviated commands, such as Stata.

Although lines of instructions should be concise, these abbreviations should not be used because:

- Less experienced readers may not recognize abbreviations.
- Abbreviations make the code harder to read, even for experienced coders.

---

## 4.2. Whitespaces and Indentations

Spaces and indentation should be used consistently and efficiently to make a program clear.

Non-indented commands should be separated by whitespaces, denoting that they are doing a different task with the dataset.

Groups of arguments associated with one instruction should be indented.

It is recommended to use **two spaces of indentation**. However, any indentation rule will be accepted if it is used consistently.

Example:

```stata
// calculate and save for with and without institutional records separately
foreach y of local inst {

  preserve

  if "`y'" == "woinst" {
    keep if private
  }

  // tabulate weighted pop counts with age groups
  egen all_count_nat_11 = total(weight)
  bysort prov: egen all_count_prov_11 = total(weight)
  bysort cma: egen all_count_cma_11 = total(weight)

  bysort age_group: egen age_count_nat_11 = total(weight)
  bysort age_group cma: egen age_count_cma_11 = total(weight)
  bysort age_group prov: egen age_count_prov_11 = total(weight)
}
```

---

## 4.3. Titles

Denote the title from the rest of the information, consistently demarking headings and subheadings.

Titles and subtitles should be used consistently throughout the entire program.

---

## 4.4. File Names

We recommend using **snake_case** in CSDUL projects.

Variables and data should be lowercase with an underscore between each word.

All new variables created or exported data should follow the same convention.

Files should also contain:

- Task name
- Date development started
- File version

Every file version corresponds to different updates made, which are kept instead of being erased or replaced.

For example:

```text
efa_pophealth_202010_01
efa_pophealth_202010_02
efa_pophealth_202010_03
efa_pophealth_202010_04
```

---

## 4.5. Names, Dates, and Contacts

Every coding file must contain:

- Start date
- Last update date
- Author's name
- Contact information

For example:

```text
================================================================
Programmer(s): Anousheh Marouzi
Contact information: anousheh.marouzi@usask.ca
Task: harmonize NHS data and calculate median income for each DA
Date started: 20th May, 2021
Last edited: 20th Oct, 2021
================================================================
```

---

## 4.6. Inputs and Outputs

Every coding file should list any files used as inputs and the files that are outputs from the process.

For example:

```text
inputs

  1. NHS - 2011 - RAW

outputs

  1. NHS - 2011 - harm
  2. NHS - 2011 - MASTER
```

---

## 4.7. Contents

The coding file should contain a table or list describing every main step performed by the code.

For example:

```text
// Contents
// 0. Setup
// 1. Make data
// 2. Tabulate point estimates with intervals
// 3. Generate figures
// 4. Control
```

---

## 4.8. Naming Variables and Functions

Variables and functions should follow consistent naming conventions that support readability, clarity, and reproducibility.

The recommended convention in CSDUL is **snake_case**:

```text
household_income
health_region
population_count
census_division
avoidable_mortality
```

---

## Reproducibility, Clarity, and Organization

How long syntax files are is usually related to clarity and "good practices."

Some authors say that a good code should not exceed 200 lines.

However, according to our experience, this depends significantly on the background and field of expertise of the analyst.

For example, in the Hub team, our codes tend to be much longer than 200 lines, but several of these lines of code are titles, subtitles, or explanations of the following line of command.

We could eliminate these lines and have a code of around 200 lines. However, we would lose clarity and the guidance that these titles and explanations provide to other users—who may be completely unfamiliar with what we are doing—and to our future selves, who sometimes wholly forget what was done and sometimes even disagree with our past version.

Instead of fixating on a specific number of lines, we advocate for code that aligns with three primary objectives:

1. **Clarity**
2. **Replicability**
3. **Organization**

While clarity and replicability have been discussed in previous sections, organization can be further elaborated.

The general organization can be the following:

1. Every syntax must start with names, dates, and contacts.
2. Set directory.
3. Harmonization of raw datasets.
4. Data processing.
5. Output generation.
6. Save results.

If all these steps are clear enough, well organized, and explained inside the syntax or with auxiliary documentation, they can be kept together.

However, if one of these steps is generic enough to be reused as part of another task, indicator generation, or model, it is strongly recommended that it be separated into another code file.

Similarly, if the length of the code is inversely proportional to its clarity and organization, it is preferable to split it into different files.

When more than one code file is needed to execute an entire process, and the order of the codes matters, the execution order must be clear.

One suggestion is to have a **Master file** that concatenates or executes the code files.

Another possibility is to provide the order in the filenames, such as:

```text
01_harmonize_data.do
02_create_variables.do
03_generate_indicator.do
04_export_results.do
```

The analyst must ensure that the organizational style is clear enough for anyone to follow.

It does not matter how clear individual code files are if their execution order is unclear.

---

## Coding Standards References

Martin, R. (2008). *Clean Code*. Pearson Education.

Naming conventions. Retrieved 13 May 2024.  
https://doc.rust-lang.org/1.0.0/style/style/naming/README.html

Wickham, H. (2021). *The tidyverse style guide*.  
https://style.tidyverse.org/index.html

---

# 5. Data Structure Standards

## Purpose

This section sets out basic data structure standards to ensure consistency across all datasets and indicators included in CSDUL.

---

## 5.1. File Formats

All data files shared must be provided in **CSV format**.

```text
.csv
```

---

## 5.2. Labels

It is recommended that the code for processing the dataset create clear and descriptive labels for all variables and observations.

Every column must have:

- A label describing the variable, including the units of measurement where applicable.
- Clear identification of any categorical variables, including definitions for each category or code used.

Providing consistent labels helps ensure that the data is understandable and usable by all stakeholders.

---

## 5.3. Variable Names

Use **snake_case** style.

All variable names and dataset names must be written in lowercase letters with an underscore (`_`) between each word.

For example:

```text
household_income
health_region
census_division
population_count
```

All newly created variables and any exported datasets must consistently follow this convention to ensure clarity and maintainability.

---

## 5.4. Dates

Use the following date format:

```text
YYYY-MM-DD
```

This corresponds to the **ISO 8601 standard**.

This format avoids confusion about the order of the day and month, making it universally readable by North American and European audiences alike.

Additionally, dates formatted this way can be correctly sorted alphabetically and chronologically.

The main date variable should be stored as a **string** to prevent format issues when importing the data into different software environments.

To further ensure compatibility, create three additional variables in numeric format:

```text
date
year
month
day
```

For example:

| date | year | month | day |
|---|---:|---:|---:|
| 2025-08-13 | 2025 | 8 | 13 |

---

## 5.5. Numeric Variables

Variables containing only numeric values must be free of any non-numeric characters.

Examples of characters that should not be included include:

```text
~
{
-
..
.
```

This ensures that when CSV files are imported into different software environments, the numeric format is preserved and values are not misread as text.

---

## 5.6. Text Variables

All text variables must:

- Be written in lowercase
- Not contain accents
- Not contain tildes (`~`)
- Not contain other special characters

This prevents inconsistencies where different software may treat identical observations as distinct due to formatting differences.

For example:

```text
québec
```

should be standardized as:

```text
quebec
```

---

## 5.7. Categorical Variables

Variables representing characteristics such as:

- Province
- Census division area
- Census metropolitan area
- Education
- Gender
- Language
- Indigenous identity
- Ethnocultural background
- Religion
- Similar demographic or geographic characteristics

must follow the classifications and coding standards established by **Statistics Canada for the Census**.

---

## 5.8. Health Regions

Use the official **Health Regions** as defined by Statistics Canada to ensure consistency and comparability in geographic health data reporting.

---

# 6. Form to Add Social Determinants to CSDUL

## Basic Information

**Date (YYYY-MM-DD):**

> [Enter date]

**Researcher (name and affiliation):**

> [Enter researcher and affiliation]

**Node Lead (name and affiliation):**

> [Enter Node Lead and affiliation]

**Indicator/Model Name:**

> [Enter indicator or model name]

---

## Purpose of the Document

This document includes several questions that must be answered by the researcher interested in adding indicators or models into CSDUL.

These questions aim to briefly explain the mathematical and theoretical framework of the indicator or model being incorporated.

The researcher must be able to answer each question clearly and concisely.

The document will be added to the model or indicator documentation in **CSDUL-OUT** and **CSDUL-RDC**.

It should serve as a quick and straightforward introduction to the indicator or model for anyone interested and provide relevant references to guide the learning process for readers.

> **If there are questions that cannot be answered because of the nature of the indicator/model, write `N/A`.**

---

## 6.1. CSDUL Environment

### Will you share the inputs through CSDUL-RDC, CSDUL-OUT, or both?

**Answer:**

> [Enter answer]

---

## 6.2. Explanation of the Indicator/Model

### 6.2.1. In simple words, explain what the indicator/model to be added consists of.

**Answer:**

> [Enter answer]

---

### 6.2.2. Are there assumptions associated with the indicator/model?

If there are, please briefly describe them.

**Answer:**

> [Enter answer]

---

### 6.2.3. How is the indicator/model derived?

Support your explanation with formulas when possible.

**Answer:**

> [Enter answer]

For example, mathematical expressions can be included in Markdown as:

```text
Y = Xβ + ε
```

or using GitHub-supported mathematical notation:

$$
Y = X\beta + \varepsilon
$$

---

### 6.2.4. What geographic unit(s) are the indicators built on?

**Answer:**

> [Enter answer]

---

### 6.2.5. How can the indicator be integrated with other datasets?

**Answer:**

> [Enter answer]

---

### 6.2.6. What are the boundaries of the indicator/model?

**Answer:**

> [Enter answer]

---

### 6.2.7. If you want to add a model to CSDUL, is this associated with a hypothesis?

If yes, describe the following.

#### a. Null Hypothesis

**Answer:**

> [Enter null hypothesis]

#### b. Alternative Hypothesis

**Answer:**

> [Enter alternative hypothesis]

#### c. Implications of Rejecting the Null Hypothesis

**Answer:**

> [Explain the implications]

---

### 6.2.8. What is the interpretation of the values of the indicator/model?

**Answer:**

> [Enter answer]

---

### 6.2.9. Potential Weaknesses

Based on the literature and your experience working with this indicator/model, is it possible to identify weaknesses in its calculations or assumptions?

To facilitate your answer, consider:

- Potential biases
- Overestimation
- Underestimation
- Omitted variables
- Endogeneity
- Dataset problems

**Answer:**

> [Enter answer]

---

## 6.3. Alternative Mathematical or Computational Versions

### Does the indicator/model have other mathematical or computational versions—not syntax—to build it?

Provide references.

**Answer:**

> [Enter answer and references]

---

### 6.3.1. Why are you building the indicator/model as proposed?

Are there advantages compared with other versions?

**Answer:**

> [Enter answer]

---

## 6.4. Potential Improvements

Do you visualize possible improvements to the indicator/model?

The upgrades can involve, among others:

- Using other datasets
- Refining calculations
- Modifying assumptions
- Changing estimation methods
- Incorporating additional information

**Answer:**

> [Enter answer]

---

# Inputs to Be Added to CSDUL

Mark the corresponding items with an `X`.

GitHub checkboxes can be completed by changing:

```text
[ ]
```

to:

```text
[x]
```

### Required/Applicable Inputs

- [ ] **Raw datasets or intermediate datasets**  
  Raw datasets or intermediate datasets that are needed to create the indicator/model.

- [ ] **Codes**  
  Codes that create the indicator/model. Be sure that your code is clear enough to be replicated in the future for yourself or any other researcher.

- [ ] **Documentation**  
  Documentation that explains step by step the entire process that builds the indicator or model.

- [ ] **Results**  
  Results consisting of the list of variables, indicators, or model results.

- [ ] **Support files**  
  These can include papers, book chapters, codes, and other supporting materials.

---

# References

Add references relevant to the indicator, model, methodology, datasets, coding procedures, or validation.

Example:

```text
Author, A. A. (Year). Title. Journal/Publisher.
https://doi.org/...
```

---

# CSDUL

The **Canadian Social Determinants Urban Laboratory (CSDUL)** provides a standardized framework for developing, documenting, validating, integrating, and disseminating social determinants of health indicators and models.

Its architecture is designed to support:

- Reproducibility
- Transparency
- Collaboration
- Data integration
- Long-term maintainability
- Research within Statistics Canada's Research Data Centres
- Public dissemination of eligible CSDUL outputs
