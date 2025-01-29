![Datafolio](./images/Presentation_Poster.png)

# Developing a Methodology for a Suicide Prevention Study

## Overview

This project focuses on analyze the quality of some datsets for analyzing and predicting suicide risk within one year after discharge among patients diagnosed with mental disorders. As the datasets were not particularly insightful, we develop a synthetic dataset in order to test the feasibility of the research, before going to collect more detailed and desirable data, wich proved to be very hard.

## Table of Contents

1. [Project Summary](#project-summary)
2. [Project Structure](#project-structure)
3. [Project Management Framework](#Project-Management-Framework)
4. [Research Questions](#Research-Questions)
5. [Data Gathering and Preparation](#Data-Gathering-and-Preparation)
6. [Stages](#Stages)
7. [Results](#results)
8. [Conclusion](#conclusion)
9. [Installation and Setup](#installation-and-setup)
10. [Usage](#usage)
11. [License](#license)

---

## Project Summary

This is an academic research project intended to serve as a practice of Big Data and Advanced Data Engineering concepts. It involves having a use case and develop a solution implementing Big Data, Data Architecture and Data Engineering technologies to solve the case using data-driven approaches and machine learning techniques.

However, the project's complexity posed a greater challenge and the datasets collected were insufficient for the large scope and the given timeframe. Realizing the situation, the goal of the project shifted from focusing on what was possible with the data available to instead design a comprehensive research framework that focused on answering the research questions with synthetic data

Despite the shortcomings, the research has yielded valuable insights into the risk factors for suicide among discharged mental health patients, including the significant role of treatment adherence, psychiatric comorbidities, and socio-economic factors.

## Project Structure

    /Suicide_Prevention_Project
    ├── /data
    │ ├── _HEALTH_HCQI_.csv                     # Incidence of suicide among people with mental health problems (OECD)
    │ ├── HEALTH_STAT_27112023140554921.csv     # Statistics of mortality by any cause (OECD)
    ├── /images
    │ ├── Barplot1.png
    │ ├── Calculation of Age-sex standardized rates and confidence intervals.jpeg
    │ ├── Lineplot1.png
    │ ├── Lineplot2.png
    │ ├── Lineplot3.png
    │ ├── SuicideIncidenceFactors.png
    ├── /Notebooks                  # Jupyter notebook for analysis and visualizations
    │ ├── Notebooks/Suicide_Risk_Analysis_Module_1_Data_Asessment.ipynb
    │ ├── Notebooks/Suicide_Risk_Analysis_Module_2_Predictive_Modeling.ipynb
    │ ├── Notebooks/Suicide_Risk_Analysis_Module_3_Predictive_Modeling_w_Synthetic_dataset.ipynb
    ├── /src
    │ ├── preprocess.py             # Data preprocessing scripts
    │ ├── ml_model.py               # Machine learning model
    │ ├── dl_model.py               # Deep learning model
    ├── REPORT_Develop_a_DataSet_for_Suicide_Prevention_.pdf
    ├── Suicide Prevention Project Strategy.md
    ├── Definitions-of-Health-Care-Quality-Outcomes.pdf
    ├── README.md                   # Project documentation
    ├── requirements.txt            # Python dependencies
    ├── LICENSE.md                  # Project licencing

---

## Project Management Framework

The **Waterfall Approach** is used for structured data preparation phases such as data preparation, ensuring compliance with healthcare regulations, and handling sensitive data. **Agile Approach** is used for dynamic iterative tasks for like data cleansing and neural network experimentation to allow flexibility, rapid development, and collaboration between data scientists and healthcare experts.

The **Cross Industry Standard Process for Data Mining (CRISP-DM)** framework was chosen for _data mining and predictive modeling_, given its robustness in handling complex data analytics projects.

## Research Questions

The project will address four main research questions:

1. **Statistical Significance of Risk Factors:** Are there statistically significant differences in suicide risk between patients with different mental disorders, and can these differences guide targeted interventions?

2. **Role of demographic and clinical indicators:** What are the key factors, including demographic variables, that contribute to the risk of suicide within one year after discharge among patients diagnosed with mental disorders?

3. **Impact of Treatment and Follow-Up Care:** How do clinical and psychosocial features (e.g., psychiatric comorbidity, treatment adherence, follow-up care) affect suicide risk after discharge?

4. **Effectiveness of Machine Learning Models in Predicting Suicide Risk:** Can machine learning models predict the risk of suicide among discharged mental health patients, and which models are most effective?

## Data Gathering and Preparation

Datasets used in this project were gathered from the **Organization for Economic Co-operation and Development (OECD)**. These datasets include information from 19 countries regarding suicide risk among patients with mental disorders. The data is available in XML format and includes a data dictionary to guide interpretation and data analysis. The dataset is available at https://stats.oecd.org/

## Stages

- **1. Domain Specific Scientific Research:** A thorough review of existing research articles, evaluating methodologies and data sources, with a focus on suicide risk among discharged mental health patients providing actionable insights for suicide prevention.

- **2. Assessing Data Storage and Management Requirements:** Develop a set of needs and resarch questions with actionable plans aimed to develop predictive modeling.

- **3. Neural Network Exploration:** Analyzing the applications, strengths, and weaknesses of different neural network types and architectures to determine the most suitable model for predicting suicide risk in the context of mental health care.

- **4. Big Data System Analysis:** An exploration of design concepts, environments, architectural patterns and technology stacks to handle large datasets, assessing the feasibility to manage, retrieve and process large datasets efficiently and in an scalable way (Big Data).

## Results

Our analysis highlights several critical insights:

- **Demographics:** Middle-aged men are at a higher risk of suicide within one year after discharge.
- **Disorder Severity:** Patients with severe mood disorders are more likely to experience suicidal ideation or attempts.
- **Treatment Adherence:** While insufficient data on treatment is available, adherence to treatment and post-discharge follow-up care are crucial to suicide prevention.
- **Temporal Risk:** The first three months after discharge represent a particularly high-risk period for patients.
- **Social Determinants:** Family support and occupational status may correlate with a lower suicide risk. However, further research is needed to investigate geographic disparities.

In order to advance more in the research, we prepared the following documents:

- Annex 1. Attributes of the population to be researched, in other words, features (columns) of the dataset to be gathered.

- Annex 2: Specific Requirements and Assessments for Data Retrieval and Processing the Big Data Datasets for this project.

- Annex 3: A not comprehensive list of the technology stack components that would be desirable in the implementation of th project

## Conclusion

While this project faced significant challenges due to its scale and complexity, it provides valuable insights into the suicide risks associated with mental health patients post-discharge. Moving forward, it is crucial to focus on improving data gathering methods, refining machine learning models, and exploring collaborative efforts to address the larger public health issue of suicide prevention.

We aim to develop a detailed plan for the future stages of this project, including dataset gathering, methodology selection, and predictive model evaluation.

### Specific Requirements and Assessments for Data Retrieval and Processing

Due to the complexity of the project, several specific requirements and assessments are necessary to ensure feasibility within the given budget and scope:

- **Data Collection:** Secure access to sensitive healthcare data, including patient information, via APIs or partnerships with institutions.
- **Data Compliance:** Ensuring compliance with healthcare data regulations, such as HIPAA, GDPR, or other local laws.
- **Big Data Architecture:** Selecting and setting up a Big Data infrastructure to handle large, dynamic datasets efficiently.
- **Machine Learning Models:** Identifying and testing machine learning models that can predict suicide risk, ensuring data quality and scalability for future analysis.

### Recommendations for improving this project

● Bias and Fairness: Beware of the potential impact of many biasing factors (in the collection and interpretation of the data, and in the extraction of conclusions) by making bias audits and fairness-aware machine learning.

● Patient engagement: Engage patients in their care by providing them with personalized insights and recommendations based on model predictions.

● Inclusion of Benefits: Collaboration with mental health professionals is essential to validate model results and ensure appropriate interventions are implemented.

● In the construction of the desired system, it may involve gathering sensitive private data, connecting to protected APIs and negotiating agreements with institutions. So, there is a set of requirements and assessments needed to ensure that the project is feasible in the budget and scope required. Each of the items in this list may involve so much detail that they may be projects in itself

---

## Installation and Setup

### Prerequisites

Make sure you have Python 3.7+ installed. You will also need to install the following libraries:

- pandas
- numpy
- scikit-learn
- tensorflow
- keras
- matplotlib
- seaborn

### Installation Steps

1.  Clone this repository:

    ```bash
    git clone https://github.com/l-maldonado/Methodology-for-a-Suicide-Prevention-Study.git
    cd sentiment-analysis-twitter

    ```

2.  Install the required dependencies:

        pip install -r requirements.txt

3.  Download the OECD datasets from the /data folder.

## Usage

**Running the Jupyter Notebook**

To explore and run the analysis, open the Jupyter notebook sentiment_analysis.ipynb located in the /notebooks folder.

        jupyter notebook

You can run each cell in the notebook to:

1. Load and preprocess the data
2. Perform sentiment analysis using different methods
3. Visualize the results

## License

All rights reserved

No Use Without Permission

No Commercial Use

Modification Prohibited

Attribution must be made

See the [LICENSE](LICENSE.md) file for details.

---
