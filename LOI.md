# Proposal

---

# Section 1: Applicant Information

## First Name

Chris

---

## Last Name

Holdgraf

---

## Email

This email address will be used for all communications and notifications about this proposal.

choldgraf@2i2c.org

---

## Organizational or Institutional Affiliation

The applicant's main organizational or institutional affiliation. Note that this may be different from the organization receiving the grant.

2i2c

---

## Country of Residence

*(dropdown — full country list)*

United States

---

## Have you ever received funding as a grantee under the CZI EOSS program?

If you were previously funded by the Chan Zuckerberg Initiative as a PI/grant lead, please select Yes. This field does not impact the evaluation of your proposal.

- (X) Yes
- ( ) No

---

## Organization Name

If the proposal is considered for funding, this will be the organization receiving the grant. Note that this may be different from the main affiliation of the applicant. You will be able to provide additional information during the Full Proposal stage, if invited to apply.

Jupyter Foundation (Linux Foundation)

---

## Organization Website

*(URL)*

https://jupyterfoundation.org

---

## Organization Country

*(dropdown — full country list)*

United States

---

## Organization Type

- ( ) Academic Institution
- (X) Fiscal sponsor
- ( ) Other Non-profit
- ( ) Industry/company
- ( ) Government

---

# Section 2: Proposal Information

---

## Proposal Title

*60 characters maximum*

Making MyST the documentation engine for AI-era bioscience

---

## Short Summary

Briefly describe the purpose of the proposal and the software project(s) it involves.

*3,000 characters maximum*

LLMs have changed the ways in which researchers learn about and use open source infrastructure. Instead of learning about a tool by Googling and following instructions, researchers rely on the information in a Large Language Model (LLM) to both learn about and generate code for their work. As the scientific community increasingly relies on LLMs, it is crucial that documentation engines also provide a structured, machine-readable foundation that LLMs can leverage to accelerate learning and discovery.

MyST (mystmd.org) is a documentation engine developed by the Jupyter Book subproject of Project Jupyter. It is the engine behind Jupyter Book, which powers over 18,000 publicly available books, courses, and knowledge bases across the sciences. MyST has an excellent foundation for LLMs, because its content is structured data by design: every MyST document includes a machine-readable JSON file to encourage re-use, interoperability, and discoverability. Where most documentation is unstructured text, from which an LLM must scrape content and infer structure, MyST content is designed to be read, traversed, and re-used programmatically.

MyST already has demonstrated adoption across the scientific community, including life-science projects like the QIIME 2 Framework, b.next bio (a synthetic biology organization, that shares their work in Devnotes), NeuroLibre (a computational preprint server), Elemental Microscopy (a computational microscopy journal). There is substantial opportunity to improve the MyST ecosystem in ways that increase the ease and power of LLM-assisted workflows. This proposal aims to make key foundational improvements in MyST's functionality in order to make it the premier documentation and communication engine for computational narratives in the age of LLMs.

To ensure that the work we do is relevant to the biosciences community, we will drive our development efforts with direct collaboration from researchers and communities in the biosciences as well as ensure that our work is compatible with developments in openRxiv's reading experience, which will be able to natively render MyST content in openRxiv Labs in 2026. The grant team already has several collaborations with researchers in the biosciences community who use the Jupyter Book and MyST Document Engines heavily. We will work with these groups to provide crucial feedback in order to drive design and development of these workflows. We'll also develop bioscience-specific documentation and directly integrate with organizations that are relevant to the biosciences community, to ensure they learn about and leverage the functionality we've created.

---

## Expected Value

If the proposal is successfully funded, what does success look like? We're seeking to understand:
- what type of capabilities the proposal is unlocking for the scientific community;
- how upstream and downstream software will be improved by the proposal;
- how the proposed work supports or implements novel functionality for AI enablement and large-scale data analysis.

*1,500 characters maximum*

Under this grant, the JupyterBook and MyST ecosystem will:

1. Improve the power and flexibility of plugin APIs to improve extensibility and support custom workflows. By significantly expanding the ways in which software can extend MyST, plugins generated by LLMs will be more reliable, efficient, and powerful.

2. Improve reproducible interactive widget support. LLMs have greatly reduced the barriers to building interactive data dashboards and visualizations, using building blocks like ipywidgets and HoloViz. Extending this functionality in MyST allows it to be a platform for rapidly creating and sharing data-driven interactive dashboards.

3. Make the computational execution engine scalable for AI workflows, connecting with other related initiatives in the JupyterHub ecosystem. By building native support for remote kernel execution, including GPU integration via JupyterHub, MyST document computation can run on cloud infrastructure that researchers already use.

Downstream, the impact of integrating computational narratives into the way that science is communicated is already changing practices and standards in scientific publishing (e.g. Notebooks Now, Open Exchange Architecture, and openRxiv Labs / Curvenote Partnership). Improving the ways that researchers can work on and communicate computational ideas — as well as publish and share them in an LLM and AI native way — is a high-profile downstream impact of investing in this work.

---

## Landscape Analysis

We are looking for proposals from software projects with demonstrated traction and adoption. Briefly describe other software tools that the audience for this proposal primarily uses (including proprietary alternatives, if they exist), and how the software project(s) in your proposal compare in terms of user base, adoption, functionality, and maturity relative to their target audience. You can add indicators of adoption and usage as needed. Please indicate if the software is used in AI applications and workflows.

*1,500 characters maximum*

Researchers writing computational documentation draw on several established tools. In scientific publishing, Sphinx is the long-standing Python documentation engine (and the Jupyter Book v1 backend) with a very large userbase; Quarto (Posit) is a feature-rich scientific publishing system spanning R and Python; Bookdown serves R Markdown books; and Observable Framework targets interactive data apps and dashboards. For general-purpose documentation, Material for MkDocs is among the most widely used Markdown engines, and Docusaurus (Meta) is a popular React-based system. A newer, AI-native category includes proprietary platforms such as Mintlify, Fern, and ReadMe. Emerging conventions include llms.txt and Context7 for exposing documentation to LLM workflows.

MyST occupies a distinct position: it is an open specification in which every document is structured data by design, shipping a machine-readable JSON representation so content, code, metadata, and cross-references can be traversed and reused programmatically rather than scraped from rendered HTML or Markdown. This makes AI-readiness intrinsic to an open, computational, scientifically grounded format. MyST is mature and widely adopted: it powers 18,000+ published Jupyter Books, with life-science users including QIIME 2, NeuroLibre, b.next, and Elemental Microscopy, and native MyST rendering coming to openRxiv Labs in 2026. It is well-positioned as a modern documentation engine built for AI-era bioscience.

---

## Software Projects to be Supported

In this section you can list up to five open source software projects that will participate in this proposal. You can add projects using the "+Create" button, and include links to their repositories.

*(subform — up to 5 entries)*

1. MyST Document Engine: https://github.com/jupyter-book/mystmd
   (Documentation and project site: https://mystmd.org)
2. Jupyter Book: https://github.com/jupyter-book/jupyter-book
   (Documentation and project site: https://jupyterbook.org)
3. JupyterHub and Binder: https://github.com/jupyterhub
   (Documentation and project site: https://hub.jupyter.org)
4. Jupyter Widgets: https://github.com/jupyter-widgets
   (Documentation and project site: https://jupyter.org/widgets)

---

## Categories

Please check up to three tags describing the type of software and its target scientific audience.

**Software type:**
- [ ] Data formats and storage
- [ ] Knowledge representation and ontologies
- [X] Scientific computing
- [ ] Statistical modeling
- [ ] Workflows and computational pipelines
- [X] Data visualization
- [ ] Interoperability
- [X] Software ecosystem infrastructure
- [ ] Hardware acceleration and scalability
- [ ] Machine learning frameworks
- [ ] Agentic frameworks
- [ ] Benchmarking and evaluation tools

**Scientific domain:**
- [ ] Genomics and transcriptomics
- [ ] Structural and molecular biology
- [ ] Cell and developmental biology
- [ ] Evolutionary biology
- [ ] Immunology
- [ ] Biological and biomedical imaging
- [ ] Bioinformatics and computational biology
- [ ] Synthetic biology
- [ ] Spatial biology
- [ ] Neuroscience
- [ ] Infectious disease and epidemiology
- [ ] Computational drug discovery
- [ ] Other

---

## Funding Track

For full instructions about the track for this call, visit the provided link.

- ( ) Track 1: Domain-specific Tools
- (X) Track 2: Foundational Libraries and Ecosystem Initiatives

---

# Section 3: PI Involvement & Policies

## Statement of PI Involvement

Confirm

---

## Policies

Confirm
