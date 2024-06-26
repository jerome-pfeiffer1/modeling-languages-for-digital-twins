# Replication package
This repository contains the replication package for the paper _Modeling Languages for Digital Twins: A Survey Among the German Automotive Industry_ by Jérôme Pfeiffer, Dominik Fuchß, Thomas Kühn, Robin Liebhart, Dirk Neumann, Christer Neimöck, Christian Seiler, Anne Koziolek, and Andreas Wortmann. 
The paper has been submitted to the practice track of  [MODELS 2024](https://conf.researchr.org/track/models-2024/models-2024-technical-track#Practice-Track).

## Data
This replication package contains all information from the survey:
- `results.csv`: A csv version of all data exported from LimeSurvey (German). Personal information from the participants has been removed. This file can be imported to reproduce the extraction results described in our paper.
- `survey_german.pdf`: The pdf version of the original survey in German.  
- `survey_german.md`: A markdown version of the original survey in German. 
- `survey_english.md`: A markdown version of the survey translated into English.
- `limesurvey_survey_222232.lss`: To reproduce our results using [LimeSurvey](https://www.limesurvey.org/de) we provide the lss export of our original survey. This can be used to redistribute our survey to new target audiences. A manual on how to import the file into LimeSurvey is described below. 

## Import a Survey into LimeSurvey
You can import a survey from the *Create, import, or copy survey* screen. 
1. From the **Surveys** dropdown options (on the top toolbar of your Limesurvey homepage) select **Import** a survey.   
2. On the Import tab, click **Browse** and choose the file you wish to import. 
3. Click the **Import survey** button. 
4. Choose the LSS files format

The import function "intelligently" re-numbers the survey, groups, questions, answers, and condition IDs so that they all match each other. No existing survey is going to be overwritten during the import process.

By default, the resource links and expression fields are also imported. Basically, the more advanced type of questions are going to be also imported along questions that include complex branching, assessments, validation, and tailoring. 

Once the import process is completed, a survey structure import summary will be displayed, showing whether it was successful or not: 


## Selection of participants and distribution
With both versions, the survey can be executed again with a different target audience in English or German. In our case we wanted to reach as much participants from diverse work areas as possible, where we invited the participants by email via an internal mailing list of 189 members of the SofDCar project.  To improve the response rate, we implemented two deadline extensions from the initial one-month-long time frame with 2 weeks of additional response time. Together with the deadline extension, we sent a mail to inform and remind the members of the consortium of the survey.

## Data extraction
In total, we had 96 participants, of which 43 completed the questionnaire. For incomplete survey responses, we took only the available answers and did not include the missing answers in our data analysis. For data analysis we utilized the commercial Tool IBM SPSS and custom python scripts.

## Research Questions 
- RQ1: How is the DT understood in the automotive industry?
    - RQ1.1: For which phases of automotive development are DTs
important?
    - RQ1.2: What are desired properties of DTs?
    - RQ1.3: What are desired purposes of using DTs?
    - RQ1.4: How do these purposes change in relation to different phases of automotive development?
- RQ2: Which modeling languages and modeling tools are currently employed in the automotive industry?
    - RQ2.1: Which kinds of models are important during automotive development?
    - RQ2.2: How important are which models in the phases of automotive development?
    - RQ2.3: Which tools are used to create and maintain these models?