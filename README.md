[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/Y4rZMh1t)
# Junior Seminar (CMPSC 580) Exemplar Project Repository

## Semester: Spring 2024

This repository contains student project materials, including project report, data, code, and references to literature for this departmentally-sponsored project. __As you complete each of the below sections in this document, please be sure to remove the preamble text so that it does not appear in your work.__ Please work with your first reader to answer any questions or concerns that you may have.

## GitHub Handle: audreyblarr

## Name: Audrey Blarr

## Major: INFM

## Project Name: Enter The Name Of Your Project

Here, think of an interesting name of the work that bring a freshness and excitement to the area of this project. Consider using a name that carries some information about what the project and provides some hint at what the project does without being too wordy.

---

## Overview

TODO (250 words minimum): Discuss the overview of the project using and building on the project description provided by the department. In this section, a concise summary is discussed of the study's key elements, offering the reader a quick understanding of the research's scope and goals. The section continues to outline the main topics, research questions, hypotheses, and /or theories in a clear and meaningful language to provide a type of roadmap for the reader to navigate the forthcoming details of the project. This section also needs to motivate the project by providing context for the study, outlining the current state of knowledge in the field, and highlighting any gaps or limitations in existing research. The section serves as a foundational guide that enables the reader to grasp the context of the study, in addition to its structure, before moving into a more technically-based discussion in the following sections of the article. In short, the "Overview" section needs to answer the `what` and `why` questions, that is `what is the project?` and `why is the project important?`

## Literature Review

TODO: Conduct literature review by describing relevant work related to the project and hence providing an overview of the state of the art in the area of the project. This section serves to contextualize the study within the existing body of literature, presenting a thorough review of relevant prior research and scholarly contributions. In clear and meaningful language, this section aims to demonstrate the problems, gaps, controversies, or unanswered questions that are associated with the current understanding of the topic. In addition, this section serves to highlight the current study's unique contribution to the field. By summarizing and critiquing existing works, this section provides a foundation for readers to appreciate the novelty and significance of the study in relation to the broader academic discourse. The "Literature Review" section further contributes to the `why is the project important?` question. The number of scholarly work included in the literature review may vary depending on the project.

## Methods

TODO: Discuss the methods of the project to be able to answer the `how` question (`how was this project completed?`). The methods section in an academic research outlines the specific procedures, techniques, and methodologies employed to conduct the study, offering a transparent and replicable framework for the research. It details the resources behind the work, in terms of, for example, the design of the algorithm and the experiment(s), data collection methods, applied software libraries, required tools, the types of statistical analyses and models which are applied to ensure the rigor and validity of the study. This section provides clarity for other researchers to understand and potentially replicate the study, contributing to the overall reliability and credibility of the research findings.

This case study will be focused around the utilization of data derived from arXiv. This information repository participates in the Open Archives Initiative (OAI), updating its data-provider nightly with metadata from new submissions. In order to perform data scraping on metadata from arXiv's OAI-PMH interface, one must abide by the rules stated in the Terms of Use for arXiv APIs (via https://info.arxiv.org/help/api/tou.html) to prevent restriction of access for their organization. The main limitation to the process of data scraping using arXiv is the rate limit, applying to all of one's devices as a collective. The limitation is stated on the information website as follows:

"When using the legacy APIs (including OAI-PMH, RSS, and the arXiv API), make no more than one request every three seconds, and limit requests to a single connection at a time."

The website also offers rules of guidance to abide by: processes you "can (and should!)" and "must not" follow while data scraping. Processes encouraged by arXiv that will be actively performed in this study include retrieving, storing, and using both descriptive metadata and content from arXiv e-prints. Tools and services will also be provided to guide readers to the e-prints containing data used and analyzed within this research, including visualizations and bibliography citations, per recommendation of arXiv. These actions will partake following the "must not do" list as well, meaning there will be no arXiv e-prints stored on the server, no faulty claims of arXiv's endorsement, and no fraudulant credentials to access the APIs. 

## Using the Artifact

TODO: The result of your work will be the delivery of some type of artifact which will likely contain software programming solutions (i.e., Python code, HTML pages, or similar). To allow the user to experience and execute your artifact, you must first explain how to set up the initial conditions to run or use the artifact. Be sure to offer explicit details and instructions regarding the installation of the necessary foundational libraries, drivers, external software projects, containers and similar types of tertiary software which are involved in executing your artifact. Once these initial software installations have been completed, then you are asked to offer the necessary instructions for actually executing the artifact. For this, please provide all command line parameters or associated bash commands for execution. Please remember that users are unwilling to "figure-out" how to use code in absence of the essential instructions concerning the execution of project artifacts.

## Results and Outcomes

TODO: Discuss the outcomes of your project in this section. Depending on the project type, the presented results and outcomes will vary. In some projects, you will be asked to present a theoretical analysis, and in others your experimental study and its results. In this section, you are also to demonstrate an enhanced version of your artifact by showing its capabilities and applications, in light of the evaluation metrics for assessing the artifact

---

## Exemplar Projects Discussions

The department's project descriptions can be found at [https://github.com/ReadyResearchers-2023-24/cmpsc-580-exemplar-projects](https://github.com/ReadyResearchers-2023-24/cmpsc-580-exemplar-projects)

## Schedule

The schedule for this work can be found at [https://github.com/CMPSC-580-Allegheny-College-Spring-2024/classDocs?tab=readme-ov-file#schedule](https://github.com/CMPSC-580-Allegheny-College-Spring-2024/classDocs?tab=readme-ov-file#schedule)

References:
https://info.arxiv.org/help/api/tou.html 

References gathered:
file:///C:/Users/akbla/Downloads/Big-Metadata-Smart-Metadata-and-Metadata-Capital-Toward-Greater-Synergy-Between-Data-Science-and-Metadata.pdf
https://www.openarchives.org/OAI/openarchivesprotocol.html
https://arxiv.org/pdf/1905.00075.pdf