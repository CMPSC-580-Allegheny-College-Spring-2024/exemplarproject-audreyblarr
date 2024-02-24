[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/Y4rZMh1t)
# Junior Seminar (CMPSC 580) Exemplar Project Repository

## Semester: Spring 2024

## GitHub Handle: audreyblarr

## Name: Audrey Blarr

## Major: INFM

## Capital in Terms of Metadata: A Framework Derived and Supported with Data Scraping 

---

## Overview

Metadata, described as "data about data", is utilized in the world of data and information by archives, libraries, and even large language models to collect and organize large amounts of data for purposes of comparison and analysis. However, it's typically assumed by data users that the development and provision of metadata is of high value, with little-to-no interrogation of exactly how the data is supplied or how it's attached to the records derived by the user. The idea of "metadata capital" has been implemented by data researchers Greenberg, Swauger, and Feinstein as a method of inspecting the value and consistency associated with metadata use based on certain "capital" concepts. The Dryad research repository is the focus of their research, where they ensure metadata quality and increase the discoverability of said data, verifying that it's "accessible, organized, intelligible, and complete to ensure ease of re-use" (via https://datadryad.org/stash/mission#our-curation-and-publication-process). Despite Greenberg’s efforts to advance the phrase “metadata capital”, it remains unclear the basis in which metadata analysis can be developed to add value, or capital, to its framework. It’s also important to note that her research is from over a decade ago, which proves to be a bit outdated. As applied to metadata, the idea of "capital" is somewhat underdeveloped; "capital" is an interdisciplinary term typically used to describe a set of information's apparent "value proposition", yet there isn't enough literature to support the claims of this proposition. Because knowledge organization is extremely economically beneficial, this study proposes three main problem statements to fill the gaps in existing research on the topic of "metadata capital": curating a consistent and cross-disciplinary definition of the word "capital" as it's applied to metadata, determining frameworks/practices that demonstrate this definition in a desirable fashion, and providing characteristics of a high "metadata capital" repository as well as how users/organizations can benefit from these repositories. To assist in answering these questions efficiently, an experiment will be conducted within this study involving data scraping of the arXiv information repository. To the returned metadata from the scraping, a developed framework of "capital" notions will be applied to specific selection criteria to investigate the extent to which the criteria is consistent to the metadata.

## Literature Review

TODO: Conduct literature review by describing relevant work related to the project and hence providing an overview of the state of the art in the area of the project. This section serves to contextualize the study within the existing body of literature, presenting a thorough review of relevant prior research and scholarly contributions. In clear and meaningful language, this section aims to demonstrate the problems, gaps, controversies, or unanswered questions that are associated with the current understanding of the topic. In addition, this section serves to highlight the current study's unique contribution to the field. By summarizing and critiquing existing works, this section provides a foundation for readers to appreciate the novelty and significance of the study in relation to the broader academic discourse. The "Literature Review" section further contributes to the `why is the project important?` question. The number of scholarly work included in the literature review may vary depending on the project.

Greenberg and her research colleagues Feinstein and Swauger were among the first to coin the term “metadata capital” in 2013-14 through their analysis of the Dryad information repository. They highlight the fact that although metadata is extremely crucial for both people and machines to find, access, and utilize information, the effectiveness of metadata can be limited by challenges such as quality, cost, and standards (via file:///C:/Users/akbla/Downloads/dcmi-952136176.pdf). Once good quality metadata is proven to be practically and beneficially reusable, the original net value of the metadata increases, promoting this concept of metadata capital. Greenberg, Feinstein, and Swauger define “capital” as commonly being an economic concept: a “topic of focus in business and operations literature that applies to impacts (net gains or losses) specific to finances, goods and services, and public needs” (citation needed). They also recognize the ability of “capital” to be utilized in other notions, such as intellectual capital (aiding profit through individual/organizational knowledge) and social capital (productive and beneficial social relationships), with the commonality between these notions being that a result or phenomenon has a specific value that has the potential of increasing over time. Because metadata capital is a product derived from both human and machine processes, and viewed as a public good, the term can fit each of the notions described, creating a great amount of opportunity for an increase of metadata capital once metadata reuse is aligned with life-cycle management of digital resources. The value of metadata increases once savings and growth are enabled through its reuse, enabling resource savings in time, labor, and financial means. Within the limitations of their study, Greenberg, Feinstein, and Swauger recognize the risk, in addition to the innovation, of coining the idea of metadata capital, as it utilizes a concept from a separate field of study and places it in the context of another. They also are upfront about the early stages of their work, meaning a full analysis of metadata quality, or cost-noting formulas, isn’t present as means of supporting their research.

Greenberg went on to publish more research articles utilizing the concept of metadata capital, pointing out in a separate resource that although metadata reuse adds value to the initial metadata cost, demonstrating a greater return on investment, cost and value aren’t always in alignment with each other (citation needed). The cost of a product may not be entirely reflective of its worth, which can be combated by extending the term “capital” in this sense to include intellectual and social capital as well as financial, as mentioned previously. Originally published in the Bulletin of the Association for Information Science and Technology, Greenberg defines “metadata capital” keeping the flexibility of the term “capital” in mind. The four different definitions she provides are as follows:

" 1. An asset that contains contextual knowledge about content. <br>
a. Content is the data or information contained in any information object (any “entity, form, or mode”). <br>
b. Context is who, what, where, when, how, why, etc., which can be captured via metadata attributes (Kunze, 2001). <br>
2. A product or service generated by human labor and/or machine-driven processes with value that increases over time or that enables the value increase of other assets. <br>
3. A good (a service facilitator) supporting a range of functions such as discovery, provenance tracking, rights management, authentication, preservation and other functions associated with lifecycle management and access. <br>
4. A public good if the product (metadata) is open, following which the services can be open. ”

Keeping these definitions in mind, Greenberg recognizes the biggest challenge with metadata valuation as the task of substantiating value. Although costs can be identified or estimated while pursuing metadata capital as a financial notion, it’s not an easy feat to determine where to begin measuring cost. Cost may start with the design of the metadata system, the builder of the system’s salary, the team implementing the workflow design, or the cost of the code library allowing this system to be built (citation needed). Evaluating the value of metadata in social and intellectual terms adds even more complexity to the matter, as it’s difficult to determine long-term consequences of metadata that may lead to discoveries several years from now.

As Greenberg’s study of metadata capital involved analysis of the Dryad data repository, this study will utilize the arXiv repository and its API technology. Hosted on arXiv.org, hundreds of thousands of e-prints can be accessed programmatically through arXiv’s API (citation needed). Beginners can access these articles through their web browser by visiting arXiv.org and browsing article listings through the links provided, or searching for specific articles by keyword(s) through a search box in the upper right hand corner of the webpage. The API is used in the exact same way as the human web interface, incorporating shortcuts to make searching by query simpler for a user. Instead of opening the web and manually searching for a [keyword], the same results can be viewed by entering in a slightly different url using this format:

http://export.arxiv.org/api/{method_name}?{parameters} (base url) <br>
http://export.arxiv.org/api/{query}?{search_query=all:keyword} (specific to search queries, where {keyword} is replaced with the keyword being searched for)

The results of the search query will look different using the API than they would on the web interface because the API returns its results in a format called Atom 1.0 rather than HTML. Furthermore, the parameters can be altered to better suit the purpose of the data search. As ‘method_name=query’, the query interface can be changed from ‘search_query’ to ‘id_list’, ‘start’, or ‘max_results’ to produce results better pertaining to the purpose of the API utilization. While ‘id_list’ produces a comma-delimited list of arXiv id’s, parameters ‘start’ and ‘max_value’ can be incorporated to download chunks of the result set at a time rather than downloading all the information at once. To further refine queries, parameter ‘sortBy’ can sort the result list by many different notions, including ‘relevance’, ‘lastUpdatedDate’, or ‘submittedDate’ to produce results pertaining more to present-time research. The ‘sortOrder’ can also be modified to sort the order of the results as either ‘ascending’ or ‘descending’. 


## Methods

TODO: Discuss the methods of the project to be able to answer the `how` question (`how was this project completed?`). The methods section in an academic research outlines the specific procedures, techniques, and methodologies employed to conduct the study, offering a transparent and replicable framework for the research. It details the resources behind the work, in terms of, for example, the design of the algorithm and the experiment(s), data collection methods, applied software libraries, required tools, the types of statistical analyses and models which are applied to ensure the rigor and validity of the study. This section provides clarity for other researchers to understand and potentially replicate the study, contributing to the overall reliability and credibility of the research findings.

This case study will be focused around the utilization of data derived from arXiv. This information repository participates in the Open Archives Initiative (OAI), updating its data-provider nightly with metadata from new submissions. In order to perform data scraping on metadata from arXiv's OAI-PMH interface, one must abide by the rules stated in the Terms of Use for arXiv APIs (via https://info.arxiv.org/help/api/tou.html) to prevent restriction of access for their organization. The main limitation to the process of data scraping using arXiv is the rate limit, applying to all of one's devices as a collective. The limitation is stated on the information website as follows:

"When using the legacy APIs (including OAI-PMH, RSS, and the arXiv API), make no more than one request every three seconds, and limit requests to a single connection at a time."

The website also offers rules of guidance to abide by: processes you "can (and should!)" and "must not" follow while data scraping. Processes encouraged by arXiv that will be actively performed in this study include retrieving, storing, and using both descriptive metadata and content from arXiv e-prints. Tools and services will also be provided to guide readers to the e-prints containing data used and analyzed within this research, including visualizations and bibliography citations, per recommendation of arXiv. These actions will partake following the "must not do" list as well, meaning there will be no arXiv e-prints stored on the server, inaccurate claims of arXiv's endorsement, or fraudulent credentials to access the APIs. 

## Using the Artifact

TODO: The result of your work will be the delivery of some type of artifact which will likely contain software programming solutions (i.e., Python code, HTML pages, or similar). To allow the user to experience and execute your artifact, you must first explain how to set up the initial conditions to run or use the artifact. Be sure to offer explicit details and instructions regarding the installation of the necessary foundational libraries, drivers, external software projects, containers and similar types of tertiary software which are involved in executing your artifact. Once these initial software installations have been completed, then you are asked to offer the necessary instructions for actually executing the artifact. For this, please provide all command line parameters or associated bash commands for execution. Please remember that users are unwilling to "figure-out" how to use code in absence of the essential instructions concerning the execution of project artifacts.

## Results and Outcomes

TODO: Discuss the outcomes of your project in this section. Depending on the project type, the presented results and outcomes will vary. In some projects, you will be asked to present a theoretical analysis, and in others your experimental study and its results. In this section, you are also to demonstrate an enhanced version of your artifact by showing its capabilities and applications, in light of the evaluation metrics for assessing the artifact

## References

TODO: References utilized in this study will be provided in this section.

---

## Exemplar Projects Discussions

The department's project descriptions can be found at [https://github.com/ReadyResearchers-2023-24/cmpsc-580-exemplar-projects](https://github.com/ReadyResearchers-2023-24/cmpsc-580-exemplar-projects)

## Schedule

The schedule for this work can be found at [https://github.com/CMPSC-580-Allegheny-College-Spring-2024/classDocs?tab=readme-ov-file#schedule](https://github.com/CMPSC-580-Allegheny-College-Spring-2024/classDocs?tab=readme-ov-file#schedule)

References:
https://info.arxiv.org/help/api/tou.html 

References gathered:
https://www.openarchives.org/OAI/openarchivesprotocol.html
https://arxiv.org/pdf/1905.00075.pdf
