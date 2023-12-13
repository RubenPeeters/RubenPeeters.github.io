---
title: "PyHBM"
excerpt: "PyHBM is a python package that was created as part of my work at VITO, to enable harmonization and FAIRification of HBM datasets."
collection: portfolio
---

## Introduction

As a data engineer, I developed a Python package that enables data harmonization in the human biomonitoring (HBM) field. The user can provide configuration in the well-known Excel format, based on simple instructions. The package can be installed and used through the command line.

## Key Points

### 1. Overview

The Python package offers a comprehensive suite of tools for data validation and transformation. Its modular design ensures flexibility, while the configuration-driven approach simplifies the customization process for users.

### 2. Features

#### a. Configurability

- Users can define data validation and transformation rules using a simple Excel file.
- Configuration supports a wide range of data types, allowing for versatile use cases.
- Intuitive syntax and template-driven approach make it accessible to users with varying levels of technical expertise.

#### b. Data Validation

- Robust data validation functionalities ensure data quality and adherence to specified criteria.
- Customizable validation rules can be easily applied based on the user-defined configuration.

#### c. Data Transformation

- Transform data based on project-specific rules and conditions.

### 3. Usage Examples

#### a. Configuration File

| Varname    | Description                                          | Type        | Unit | MissingsAllowed | MinValue | MaxValue | AllowedValues                                                                                   | DecimalsAfterComma | Conditional                                 | Formula | Remarks |
|------------|------------------------------------------------------|-------------|------|-----------------|----------|----------|-------------------------------------------------------------------------------------------------|--------------------|---------------------------------------------|---------|---------|
| id_subject | UID of the subject                                   | integer     |      | 0               | 1        | inf      |                                                                                                 |                    |                                             |         |         |
| height     | height of the subject at sampling                    | decimal     | cm   | 1               | 30       | 250      |                                                                                                 | 1                  |                                             |         |         |
| isced      | Highest education level of the subject (ISCED scale) | categorical |      | 1               |          |          | 1 = Low education (ISCED 0-2); 2 = Medium education (ISCED 3-4); 3 = High education (ISCED >=5) |                    | IF ageyears IS < 20 THEN isced IS not empty |         |         |


#### b. Data

| id_subject | height | isced |
|------------|--------|-------|
| 1          | 160    | 1     |
| 2          | 170    | 2     |
| 3          | 180    | 3     |

#### c. Usage (validation)

```bash
> pyhbm data/file.xlsx -cb config/codebook.xlsx
```
With additional flags for output paths (`-o`) and levels of logging output (`-v`, `-vv`).

#### d. Output

```bash
{
    "structural": [],
    "validation": [],
}
```

The output is in JSON format, separating structural and validation errors.



## Relevant technologies

- Languages: 
  - Python
- Libraries:
  - pandas
  - numpy
  - scipy
  - typer
  - simplejson
  - rdflib
  - rich
  - pytest
  - pytest-cov
  - Faker
  - hypothesis
  - mkdocs
  - ipykernel
- Other
  - black
  - flake8
  - isort
  - pydocstyle

## Relevant links

The package is used in an online tool, which you can find here:
- https://tools.hbm.vito.be/validation

Additional information on the harmonization process that is enabled through the package can be found here:
- https://hbm.vito.be/tools/data-harmonization
