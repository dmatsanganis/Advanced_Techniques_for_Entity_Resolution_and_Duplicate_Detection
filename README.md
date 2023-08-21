# Advanced Techniques for Entity Resolution and Duplicate Detection

This repository is dedicated to the exploration and analysis of the intricate domain of entity resolution with a specific emphasis on duplicate detection. Throughout the document, various advanced methodologies have been used to ensure data precision and uphold data integrity.

In the realm of data management and analysis, maintaining data quality is of paramount importance. Duplicate entries within datasets can lead to skewed results and erroneous insights. The process of entity resolution involves identifying and consolidating duplicate records that correspond to the same real-world entity. This notebook explores advanced techniques for achieving accurate entity resolution and duplicate detection, utilizing two sophisticated methodologies: **Token Blocking and Meta-Blocking**.


## Key Sections

1. **Token Blocking for Block Creation**: This section focuses on the Token Blocking approach, a schema-agnostic method, as a strategy for block creation.

2. **Jaccard Similarity with Emphasis on Title**: Titles often encapsulate the primary essence of entities. This section explores the significance of the 'title' attribute of entities and employs the Jaccard Similarity Function to determine how these titles align and contribute to the entity resolution process.

3. **Discussions and Methodologies**: Various strategies and methods are explored in detail throughout the document, providing insights into the decision-making process and analytical reasoning behind each choice.


## In this repository you can find

- **Documentation Report**: An in-depth document elucidates the methodology, findings, and implications. It serves as a comprehensive guide for readers to grasp the importance of the entity resolution process.

- **Analysis Jupyter Notebook**: A practical accompaniment to the documentation, this Jupyter Notebook contains the actual code implementation and analysis. Developed using Python 3.10, the notebook offers a hands-on view of the techniques described, allowing readers to dive into the coding and analytical practices employed.


## Notebook Overview
The provided repository's Jupyter notebook is structured to address the following tasks:

### Task A: Token Blocking for Block Creation
In this section, we delve into Token Blocking, a schema-agnostic approach that generates blocks using Key-Value (K-V) pairs. These pairs encapsulate distinct Blocking Keys (BKs), derived from entity attribute values. The id column is excluded from the process to ensure precision. Transforming attribute strings to lowercase during token creation minimizes mismatches. The outcome is an index of comprehensive BKs, elegantly presented using a function designed for clear Key-Value pair visualization. 

### Task B: Calculating All Possible Comparisons
Task B involves computing all possible comparisons essential for resolving duplicates within the established blocks from Task A. By quantifying the total number of comparisons, we gauge the computational complexity of the duplicate detection process, paving the way for efficient and accurate entity resolution.

### Task C: Constructing a Meta-Blocking Graph with CBS Weighting
In Task C, we introduce Meta-Blocking, a strategy where a graph is constructed based on the block collection from Task A. We employ the CBS (Common Block Scheme) Weighting Scheme to optimize the graph's efficacy. Pruning edges with weights below 2 refines the block collection, minimizing unnecessary comparisons. The pruned collection becomes the foundation for recalculating the final number of comparisons.

### Task D: Jaccard Similarity Function for Attribute Comparison
The final task introduces a custom function designed to assess the Jaccard similarity between entities based on the "title" attribute. Although the function doesn't perform actual comparisons within this notebook, it serves as a valuable tool for measuring similarity in attribute values.

Through this notebook, readers will gain proficiency in advanced techniques for entity resolution and duplicate detection. By utilizing real-world data and following step-by-step instructions, participants can enhance their data manipulation skills and contribute to better data quality and accuracy.

## Note
Please note that while this notebook comprehensively addresses each task with explanations and code implementations, it is an integral part of a broader analysis. **The notebook is accompanied by a separate PDF documentation file, providing a contextual framework and supplementary insights to augment the understanding of the intricate entity resolution process**.

## Contributors

- [x] [Dimitris Matsanganis](https://github.com/dmatsanganis)



![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
