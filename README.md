# Automatic Ontology and Knowledge Graph Construction with LLM

This repository contains code, data, prompts and results related to the (semi-)automatic pipeline of  Ontology and Knowledge Graph Construction with Large Language Models (LLMs).

## Overview

In this project, we explore the potential of utilizing Large Language Models (LLMs) for the generation of Knowledge Graphs (KGs). This work explores the (semi-)automatic construction of KGs facilitated by open-source LLMs. Our pipeline involves formulating competency questions (CQs), developing an ontology (TBox) based on these CQs, constructing KGs using the developed ontology, and evaluating the resultant KG with minimal to no involvement of human experts. We showcase the feasibility of our semi-automated pipeline by creating a KG on deep learning methodologies by exploiting scholarly publications. To evaluate the answers generated via Retrieval-Augmented-Generation (RAG) as well as the KG concepts automatically extracted using LLMs, we design a judge LLM, which rates the generated content based on ground truth.
The repository encompasses various components including code for data preprocessing, prompts used for LLMs, datasets employed in experiments, and the corresponding results obtained.

## Contents

* Code/: Contains code files for data preprocessing, Competency questions, ontology and KG generation, and evaluation of KGs.
* CQs/: Contains the competency questions generated by the LLM.
* SOTAOntologies/: Contains the state-of-the-art ontologies for reuse for the creation of DLProv Ontology
* Ontology/: Contains the DLProv Ontology generated by LLM and saved in Protege.
* Data/: Contains datasets used in experiments, including scholarly publications and competency question answers.
* Prompts/: Includes prompts utilized for directing LLMs in generating competency questions, ontology and KGs.
* KG_files/: Contains the results obtained from the experiments, including generated KGs.
* Evaluation/: Contains the evaluation results, including evaluation of competency questions and KGs.

## Usage
Add the Hugging face access token in the helper_functions.py in the following line:
access_token_read = os.getenv('access_token_read_hf')  

Install the prerequisite using the requirements.txt file. 

To run the whole pipeline, submit (execute) your job using main.py and use config.ini to customise the variables and paths 

## License
The repository is licensed under [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).

## Publication
Kommineni, V. K., König-Ries, B., & Samuel, S. (2024). From human experts to machines: An LLM supported approach to ontology and knowledge graph construction. arXiv preprint arXiv:2403.08345. 
[https://doi.org/10.48550/arXiv.2403.08345](https://doi.org/10.48550/arXiv.2403.08345)
