\# Robust Rumor Detection on the PHEME Dataset



This repository contains the research code and experimental implementation supporting the IEEE research paper on robust rumor detection using textual representations, user-credibility features, and propagation-aware graph neural networks.



\## Overview



The study investigates rumor detection on the PHEME dataset by combining:



\- RoBERTa-based source-tweet representations

\- User-credibility features

\- Graph Convolutional Networks (GCN)

\- Bidirectional Graph Convolutional Networks (Bi-GCN)

\- DropEdge-based graph regularization

\- Temporal and early-detection evaluation

\- Leave-One-Event-Out (LOEO) evaluation

\- Feature ablation studies

\- Statistical significance testing



The repository provides the experimental notebook used to implement and evaluate the proposed models and experimental settings reported in the accompanying paper.



\## Repository Structure



```text

PHEME-Rumor-Detection/

│

├── MBasit\_PHEME\_IEEE\_Reproducibility.ipynb

├── requirements.txt

├── README.md

├── .gitignore

└── .gitattributes



Dataset



The experiments use the PHEME dataset for rumor detection.



The dataset is not included in this repository. Users should obtain the dataset from its original source and place the required files in the appropriate local data directory before running the notebook.



Methodology



The experimental pipeline combines textual and propagation-level information.



Text Representation



RoBERTa is used to obtain contextual representations of source tweets.



User-Credibility Features



The framework incorporates user-level credibility information alongside textual representations.



Graph-Based Modeling



Conversation propagation structures are represented as graphs and evaluated using graph neural network architectures, including GCN and Bi-GCN.



Robustness and Generalization



The experiments include:



Standard train/test evaluation

Leave-One-Event-Out (LOEO) evaluation

DropEdge regularization

Temporal snapshots

Early-observation settings

Feature ablations

Statistical significance analysis

Experimental Reproducibility



The main implementation is provided in:



MBasit\_PHEME\_IEEE\_Reproducibility.ipynb



The notebook contains the data-processing pipeline, feature construction, model implementations, training procedures, evaluation procedures, ablation experiments, and statistical analyses used in the study.



A fixed random seed and documented experimental configurations are used where applicable.



Exact numerical reproduction may depend on the software environment, package versions, hardware, and availability of the original dataset.



Requirements



The main Python dependencies are listed in:



requirements.txt



A Python environment with Jupyter Notebook support is recommended.



Install the dependencies using:



pip install -r requirements.txt



PyTorch Geometric may require installation instructions specific to the installed PyTorch version and operating system.



Running the Experiments

Obtain the PHEME dataset from its original source.

Prepare the dataset according to the structure expected by the notebook.

Create a Python environment with the required dependencies.

Install the packages listed in requirements.txt.

Launch Jupyter Notebook:

jupyter notebook

Open:

MBasit\_PHEME\_IEEE\_Reproducibility.ipynb

Run the notebook sections in order.

Reported Experiments



The notebook includes the experimental settings discussed in the paper, including:



RoBERTa-based baseline evaluation

RoBERTa with user-credibility information

GCN and Bi-GCN models

DropEdge experiments

Temporal evaluation

Early-detection evaluation

Feature ablations

Leave-One-Event-Out evaluation

Clean event-subset analysis

Statistical significance testing

Data and Generated Files



The dataset and large generated artifacts are intentionally excluded from this repository.



The .gitignore file excludes common dataset archives, cached embeddings, model checkpoints, and generated experiment artifacts.



Paper



This repository supports the accompanying IEEE research paper.



The final bibliographic citation will be added after publication.



Code Availability



The source code and experimental implementation are provided to support transparency and reproducibility of the reported research results.



License



A repository license will be added when the appropriate licensing terms for the research code have been determined.

