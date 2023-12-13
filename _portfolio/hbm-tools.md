---
title: "HBM tools"
excerpt: "The HBM tools website exposes the functionality of PyHBM, in a GDPR-friendly way.<br/><img src='/images/hbm-tools.png'>"
collection: portfolio
---

## Description

In the human biomonitoring (HBM) field, data is inherently sensitive. Hence, why we exposed the python functionality of the PyHBM package through a web-tool that runs locally. The python code is compiled into WebAssembly, allowing it to be run in the user's computer. This ensures data confidentiality.

## Usage

1. Selecting a codebook

First you will have to select the relevant `codebook` (later on you will be able to upload your own). `codebook` is just another word for the configuration.
![select-codebook](/images/select-codebook.png)

1. Selecting a file

With the select file button, you will select the data you want validated, according to the codebook you selected.

3. Validate

After selecting your file, the data will be validated automatically. Errors that have been found will be written to the screen, as seen below.

![validation-output](/images/validation-output.png)

## Relevant technologies

- Languages: 
  - JavaScript
- Libraries:
  - React
  - React Syntax Highlighter
  - TailwindCSS
  - MaterialUI
- Other
  - Pyodide

## Relevant links

Information on the development of PyHBM can be found here:
- [PyHBM](https://rubenpeeters.github.io/portfolio/pyhbm/)

The tools can be found here:
- [HBM tools](https://tools.hbm.vito.be/)

Additional information on the harmonization process that is enabled through the tools can be found here:
- [Data harmonization guide](https://hbm.vito.be/tools/data-harmonization)


