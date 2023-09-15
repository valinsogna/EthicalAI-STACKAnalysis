# STACK Student Response Analysis for Sage Foundation Ethical AI Hackathon
A ML algorithm capable of conducting an in-depth analysis of students' responses to [STACK](https://stack-assessment.org/) questions for the Ethical AI Hackathon promoted by [Sage Foundation](https://www.sage.com/en-us/company/sage-foundation/). 

STACK is the world-leading open-source online assessment system for mathematics and STEM. It is available for Moodle, ILIAS and as an integration through LTI.

The algorithms used were **CA for discovery lexical similarity between students' incorrect answers** and **K-means to cluster them**.

## Table of Contents
1. [Team Introduction & Understanding the Problem](#team-introduction)
2. [Data Cleaning](#data-cleaning)
3. [Python Scripts & Visualisation](#scripts-and-visualisation)
4. [ML algorithms](#ml-algorithms)
5. [Presentation](#presentation)

## 1. Team Introduction & Understanding the Problem <a name="team-introduction"></a>
### Review of the sample data
* [Link to Sample Data](https://docs.google.com/spreadsheets/d/1lKqZ2Zz76gLx_kFqmoE8V4eDIg5wUbPf/edit#gid=1487606072)

### Hackathon Challenge
Our challenge in this hackathon is to develop a machine learning algorithm to analyze students' responses to STACK questions. The aim is to classify correct vs. incorrect responses, further delve into the types of incorrect responses, group similar incorrect responses, and identify any outlier responses.

### Aim
To devise an algorithm that effectively provides an in-depth analysis of students' answers to STACK questions.

### Specific Objectives
1. **Classification of Correct vs. Incorrect Responses**  
2. **Multilevel Classification of Incorrect Responses (Predicted vs. unpredicted responses using PRT paths)**
3. **Cluster Analysis - Grouping Similar incorrect responses**
4. **Anomaly Detection Based on Question Text**

## 2.Data Cleaning <a name="data-cleaning"></a>
For the purposes of our analysis, only the finished attempts are considered.
* [Link to Data Cleaning Script](<your_link_here>)

## 3. Python Scripts & Visualisation <a name="scripts-and-visualisation"></a>
Each objective was approached with a dedicated Python script, followed by visualization to represent the analysis results.

### Writing Python Scripts
1. **Script for Objective 1-2**: [Link to the Code](<your_link_here>)
2. **Script for Objective 3-4**: [Link to the Code](<your_link_here>)

## 4. Machine Learning Analysis Summary <a name="ml-algorithms"></a>
- **Contingency tables**: for each type of question, a contingency table of students'answer was build using as vocabulary the characters present in each response.
- **Correspondence Analysis (CA)**: for each type of question, 2D CA was performed on predicted and not predicted wrong students'answers in order to analyzes lexical (dis)similarities between them.
- **K-means**: used for clustering to understand common errors for each type of question, using as input the results from each CA.
- **Data Saving and Retrieval**: save analyzed data for future use or further analysis.

## 5. Presentation <a name="presentation"></a>
The findings, algorithm, and insights were compiled and documented for presentation to the Hackathon judges.
* [Link to PPT Presentation](<your_ppt_link_here>)

### Future Improvements
* After individual testing, all code blocks should be integrated into a single program.
* Increase num of dimensions for Correspondence Analysis (3D).
* Add mathematical functions and symbol to the vocabulary for creating contingency table.
* Choose effective num of clusters based on the better view of data from 3D CA.
* **Create API to fetch this clustering data and work as an input to the STACK system**.

## Team & Researchers
Below are the contributors to this project:
### Team Members
- **Umang Murawat**: [LinkedIn](www.linkedin.com/in/umangmurawat) team-leader
- **Gaurav Khetwal**: [LinkedIn](https://www.linkedin.com/in/gaurav-khetwal-967b03157/)
- **Navjot Singh**: [LinkedIn](https://www.linkedin.com/in/navjot-singh-b5147b84)
- **Davinder Singh**
- **Jivan Goyal**

### Lead Researchers
- **Valeria Insigna**: [LinkedIn](https://www.linkedin.com/in/valeria-insogna-05468a1a7/)
- **Zuma Zevick**: [LinkedIn](https://www.linkedin.com/in/juma-zevick-591241291/)
- **George Osang**

## References
- **Google Colab**: [https://colab.research.google.com]([https://colab.research.google.com](https://drive.google.com/drive/folders/1ydydOYnVIOt2A6L7Qwhs_Jlwhi2tESBB))
- **Prince for Correspondence Analysis**: [https://pypi.org/project/prince/](https://pypi.org/project/prince/)
- **Plotly for Interactive Plots**: [https://plotly.com/python/](https://plotly.com/python/)
- **KMeans Clustering**: [https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html)
