---
layout: archive
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Description

Aspiring polymath with a formal education in Information Engineering Technology. Interested in AI/ML, knowledge graphs, ontologies, semantic annotation, FAIR data, and their application across various domains. Ask me about my experience at VITO and the many challenges we are conquering there. Avid lover of games, both online and over the board.

## Education

- Bachelor of Science in Information Engineering Technology (2016-2021)
	- Bachelor project: "Development of a code learning platform for kids, through block programming"
- Master of Science in Information Engineering Technology (2021-2022, Cum Laude)
	- Master thesis: "Deep reinforcement learning for network intrusion detection"

## Work Experience
- Data Engineer at VITO, Health Unit (2022 - present).
	- Relevant skills:
		- Data engineering
		- Data governance
		- Data stewardship
		- FAIR data	
		- Project management
		- Writing research output
		- Linked data
		- Ontologies
	- Projects:
		- PARC
			- https://www.eu-parc.eu/
			- *"Partnership for the Assessment of Risks from Chemicals aims to develop next-generation chemical risk assessment to protect human health and the environment. It supports the European Union's Chemicals Strategy for Sustainability and the European Green Deal's “Zero pollution” ambition with new data, knowledge, methods and tools, expertise and networks."*
			- Position in project: data engineer/researcher as part of WP7 - FAIR data
			- 200+ partners in over 80 countries. 400 million EURO in funding.
			- Responsibilities:
				- Developing python package that allows validation of data, adding of calculated variables and calculating summary statistics. The package also allows for transformation to FAIR data format, namely RO-crate. The configuration for this package can be created by the researcher itself through the use of an excel format.
				- Developing web tool which exposes this functionality to the less-technical user. (https://hbm.vito.be and https://tools.hbm.vito.be). The tool is not allowed to use a backend, due to the highly-sensitive nature of the data. The python package is compiled to WebAssembly using Pyodide.
				- Further developing existing data platform, for storage of Personal Exposure & Health (PEH) data.
				- Leading workshops to harmonize metadata for the Human Biomonitoring (HBM) domain. Participants are domain experts, with little technical expertise. 
				- Transforming metadata to FAIR data, by linking to FAIR ontologies and FAIR controlled vocabularies.
				- Leading FAIRification of *model* metadata, such as metadata on PBK model inventories. (deliverables to make FAIR: [AD6.3](https://www.eu-parc.eu/sites/default/files/2023-08/PARC_AD6.3.pdf), [AD6.4](https://www.eu-parc.eu/sites/default/files/2023-08/PARC_AD6.4.pdf))
				- Contributing to FAIR ontologies developed in PARC [parco](https://github.com/eu-parc/parco)
				- Contributing to conceptual model to capture research data. Started based on HBM data. [parco-hbm](https://github.com/eu-parc/parco-hbm)
				- Contributing to conceptual models of aggregate exposure [aggregate-exposure-modelling](https://github.com/eu-parc/aggregate-exposure-modelling)
				- Developing script to create FAIR convergence matrix [FAIR convergence matrix](https://github.com/eu-parc/FAIR-convergence-matrix)
				- Following FAIR courses. These are given by the GO Fair Foundation (GFF). After finishing the course, the students become FAIR facilitators and get the responsibility of taking over the tasks of the GFF for the remaining duration of the project. I have completed this course and will get my official certification on 29th january 2024. Further courses are in progress. They will lead to a FAIR trainer certification. [GFF](https://www.gofair.foundation/)
				- Harmonizing questionnaires across all partners.
					- Developing data template which handles complexity of both the links between questions and the additional validation.
			- Relevant technologies:
				- Python
					- Pandas
					- Numpy
					- Scikit-learn
					- dataclasses
					- Jupyter
					- Packaging
					- Typer
					- MKDocs
					- Poetry
					- Anaconda
				- JavaScript
					- React
					- Tailwind
					- MaterialUI
				- RDF
				- Turtle
				- XML
				- JSON
				- Linked data
				- RO-crate
				- Ontologies
					- OWL
					- OBI
					- And many domain-specific ontologies such as ENVO
				- Docker
				- Jenkins
				- Atlassian products:
					- BitBucket
					- Confluence
					- Jira
				- GitHub
				- Ubuntu
					- Bash
				- Windows
					- PowerShell
		- INQUIRE
			- https://inquire-he.eu/
			- "*Enabling homes to realise zero pollution holds multiple health benefits for all Europeans – especially our children. This is the goal of the EU-funded INQUIRE project. It will provide the knowledge, tools and measures needed to significantly enhance indoor air quality. Research on hazardous determinants and their sources, risk factors and effects will focus in particular on infants and young children up to 5 years old. The work will include non-invasive sampling and monitoring of over 200 homes in eight countries over the course of 1 month. Results will inform evidence-based recommendations and support beneficial exploitation by industry and policymakers.*"
			- Position in project: data engineer/researcher as part of WP6 - FAIR data
			- Responsibilities:
				- Analyzing and assessing of FAIR repositories, for storage of project data.
				- Development of data platform for storage of *PEOPLE* and *HOME* data (INQINT).
					- This platform was split between Mazaryk University (HOME) and VITO (PERSON), which added more complexity.
					- Additionally, because data was separated into PEOPLE and HOME, extra care had to be taken with regards to GDPR. The data might not be identifiable when separated into those two databases, but might be when they are merged together.
				- Further developing python package to be able to handle environmental (HOME) data.
				- Gathering, developing and harmonizing metadata for all data flows in the project.
			- Relevant technologies:
				- INQUIRE and PARC overlap quite a lot. The relevant technologies are quite the same.
		- EIRENE
			- https://www.eirene-ri.eu/
			- "*Environmental Exposure Assessment Research Infrastructure (EIRENE) aims to fill the gap in the European infrastructural landscape and to pioneer the first EU infrastructure on human exposome. EIRENE RI was designed as a geographically balanced network of distributed research infrastructures.*"
			- Position in project: Data engineer
			- Responsibilities:
				- Main developer of the research infrastructure
				- This project is very much still in the conceptual phase. Only an architecture has been thought out.
			- Relevant technologies:
				- None as of yet
	- Non-project related, or additional:
		- Internal NLP project on semantic similarity between questionnaires.
			- Description: "*Harmonizing questionnaires based on semantic similarity as to reduce the manual work of researchers. This allows for searching over historical datasets/studies with improper description. Results become comparable.*"
			- Responsibilities:
				- Solo developer of all code related to the NLP project.
			- Relevant technologies:
				- Python
					- Spacy
					- NLTK
					- Gensim
					- scikit-learn
					- polyglot
		- Data management team:
			- Description: "*My colleague and I were the first technical people in the unit. As our team started growing we needed some kind of hierarchy. My colleague, who is my senior by 25 years, has lots of content-related knowledge, but refrains from leading the team. This led to him and myself taking on this work together.*"
			- Responsibilities:
				- Managing colleagues.
				- Matching problems with skillsets of colleagues.
				- Making sure we make deadlines.
				- Managing expectations.
			- Relevant skills:
				- Verbal and written communication
				- Active listening and collaboration
				- Critical thinking and analytical skills
				- Decision-making and time management
				- Leadership, delegation, and prioritization
				- Conflict resolution and empathy
				- Innovation and handling pressure
				- Patience, relationship building, and professional networking
				- Self-awareness
		- Part of VITO Data Ambassador team
			- Description: "*The VITO Data Ambassadors are data-minded individuals, chosen as representatives for each unit to translate the needs of the unit to a VITO-wide level.*"
			- Responsibilities:
				- Translate knowledge of the unit to VITO Data Governance Board.
				- Attending conferences regarding Data Governance.

## Certifications or Training

- Software Development Mindset by ArjanCodes
- FAIR Facilitator Training by Go FAIR Foundation

## Extracurricular Activities or Leadership Roles

- Founder of UGent Esports, an esports organization for Ghent University students with over 300 members, winning notable tournaments.
	- Relevant skills:
		- Leadership
		- Organizational skills
		- Patience, relationship building
- Creation of discord bot for managing UGent Esports
	- Relevant technologies:
		- Python
			- discordpy
			- numpy
			- pandas
- Creation of discord bot to explore the possibilities of python. The bot exposes this functionality to users. At one point in time, this had over 100.000 users. (https://github.com/RubenPeeters/Itachi)

## Languages

- Dutch (native)
- English (proficient)
- French (basic)
- German (basic)
