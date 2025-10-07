**OHDSI Methods Working Group (Feature Selection & GIS Extension)**

**Introduction**

The OHDSI Methods Working Group (WG1) is dedicated to advancing methodological innovation within the OHDSI ecosystem, focusing on feature extraction and reproducible workflows for machine learning applications on OMOP CDM data.

This WG provides a collaborative space for low-code/no-code approaches to feature engineering, making sophisticated methods accessible to a wider community of clinical, population health, and environmental health researchers. By integrating OMOP CDM with environmental and SDoH data through the OHDSI GIS Extension, the WG enables exposome research at scale.

Our work is part of the OHDSI Methods Library (HADES) and connects with broader FAIR, open science, and metadata catalog initiatives.

**Objectives**

- Develop standardized feature extraction pipelines that generate covariates from OMOP CDM datasets.
- Support low-code/no-code ML platforms by creating workflows that move seamlessly from feature extraction → RAutoML pipelines.
- Extend OMOP CDM with an external_exposures table, integrating climate, toxicant, and social determinants of health data through the GaiaCatalog.
- Document datasets and workflows using Schema.org and JSON-LD, ensuring FAIR alignment, discoverability, and reuse.
- Explore the potential of LLMs trained on FAIR metadata catalogs to enhance dataset search and discovery.

**Activities**

- **Feature Extraction**

Using HADES tools and complementary R packages to generate covariates from OMOP CDM.

Designing workflows that are reproducible and portable across datasets and research contexts.

The WG maintains a dedicated no-code/low-code test environment on GitHub: [aphrc-nocode/test-doc-env](https://github.com/aphrc-nocode/test-doc-env)  
One highlighted project is Advanced Feature Selection, which:

Extracts candidate predictors from OMOP CDM and this project forms part of a larger pipeline where feature extraction is then handed off to low-code/no-code ML environments for model development.

- **GIS Extension & Exposome Research**

GaiaCatalog hosts climate, toxicant, and SDoH datasets.

Data are staged, harmonized, and spatiotemporally joined to OMOP CDM.

A new external_exposures table captures each person's exposome, enabling cross-domain research.

Actively collaborating with metadata catalog initiatives, including:

- eLwazi
- World Bank Metadata Editor
- Schema.org Dataset Catalogs
- The Dakar (Senegal) and Douala (Cameroon) air pollution health risks assessment WG
  - The Dakar (Senegal) and Douala (Cameroon) air pollution health risks assessment WG is building a data warehouse staging database with fact tables and dimensions for satellite and ground sensor observations
  - It includes a service that produces GaiaCatalog entries on demand as an entry point into the GIS extension and OMOP CDM instances maintained by pathfinders and HDSS sites across the continent.
  - This project is growing the OHDSI GIS extension with vocabularies used in the description of aggregates (aka statistical variables) for external exposures as specified by the WHO, Africa CDC and other international research and response organizations

Experimenting with AI-assisted catalog search, training LLMs on FAIR datasets to enhance metadata-driven discovery.

**Membership & Roles**

- **Mentor (Jay Greenfield):** Provides strategic oversight, ensures alignment with OHDSI's broader mission, and mentors the WG team.
- **Facilitator:** Coordinates WG activities and community engagement.
- **Design & Development Lead (Letisha):** Leads feature extraction and supports the no-code/low-code pipeline.
- **OMOP CDM Expertise (Dora):** Ensures methodological alignment with CDM standards.
- **Contributors:** Community members co-designing and co-developing workflows, documentation, and methods.

**Outputs & Future Directions**

- A library of standardized methods for feature extraction integrated into HADES.
- A validated external_exposures OMOP CDM table supporting exposome research.
- A metadata-rich catalog of datasets documented with Schema.org and JSON-LD.
- An open repository of feature extraction and selection workflows, accessible through the no-code/low-code platform.
- Papers and guidelines on best practices for reproducible feature engineering.
- Cross-disciplinary collaborations linking clinical, environmental, and computational research.

**Ways of Working**

- Open collaboration: All discussions and documentation are shared via GitHub and Discord.
- Iterative development: Start simple, test often, and refine through community feedback.
- Integration-first mindset: Ensure compatibility with existing OHDSI standards (HADES, OMOP CDM).
- Capacity building: Provide opportunities for learning and co-development, especially for researchers in LMICs.
- FAIR principles: Commit to findable, accessible, interoperable, and reusable methods and data.

**Communications & Community Platforms**

A Discord workspace has been established and is maintained by the OSPO Now team for the DSWB community. It offers lightweight, real-time communication through instant messaging and audio calls, complementing GitHub and other channels.

Within this workspace, the #ohdsi-methods-wg channel is the dedicated space for our working group. It supports:

- Learning and discussion on feature extraction methods using HADES.
- Sharing resources, asking questions, and coordinating development efforts.
- Collaboration around extending OMOP CDM with environmental and exposome data.

Other relevant channels in the DSWB Discord include:

# introduce-yourself (new member welcomes),

# community-guidelines (code of conduct),

# general (community calls and events),

# dataset-documentation (Schema.org/JSON-LD practices), among others.

Discord is complemented by:

A WhatsApp group (maintained by APHRC) for reminders and quick posts.

A LinkedIn page for sharing external updates and boosting the visibility of WG activities.

These tools together create an inclusive, multi-channel communication ecosystem supporting WG collaboration

This WG is building the bridge between OMOP-based data science and machine learning, empowering a wider community of researchers to engage in high-quality, FAIR-aligned, and reproducible science.
