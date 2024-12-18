# [Building an ML Pipeline]()

## [Demo]()
This project will utilize a dataset that features characteristics of bone marrow transplants specifically for pediatric patients, sourced from UCI’s Machine Learning Repository. The goal is to create a comprehensive pipeline that encompasses all necessary preprocessing and data-cleaning procedures, followed by the selection of the most effective classifier to forecast patient survival outcomes.

### Scenario
The dataset focuses on pediatric patients suffering from various hematologic conditions, including both malignant disorders such as acute lymphoblastic leukemia, acute myelogenous leukemia, chronic myelogenous leukemia, and myelodysplastic syndrome, as well as nonmalignant cases like severe aplastic anemia, Fanconi anemia, and X-linked adrenoleukodystrophy.

All patients underwent unmodified allogeneic hematopoietic stem cell transplantation from unrelated donors. This study aimed to pinpoint the key factors that contribute to the success or failure of the transplantation process, specifically testing the hypothesis that a higher dosage of CD34+ cells per kilogram could enhance overall survival rates while minimizing adverse effects that might compromise the patients' quality of life.

**Features**

- Recipientgender - Male - 1, Female - 0,
- Stemcellsource - Source of hematopoietic stem cells (Peripheral blood - 1, Bone marrow - 0),
- Donorage - Age of the donor at the time of hematopoietic stem cells apheresis
- Donorage35 - Donor age <35 - 0, Donor age >=35 - 1
- IIIV - Development of acute graft versus host disease stage II or III or IV (Yes - 1, No - 0),
- Gendermatch - Compatibility of the donor and recipient according to their gender (Female to Male - 1, Other - 0),
- DonorABO - ABO blood group of the donor of hematopoietic stem cells (0 - 0, 1, A, B=-1, AB=2),
- RecipientABO - ABO blood group of the recipient of hematopoietic stem cells (0 - 0, 1, A, B=-1, AB=2),
- RecipientRh - Presence of the Rh factor on recipient�s red blood cells ('+' - 1, '-' - 0),
- ABOMatch - Compatibility of the donor and the recipient of hematopoietic stem cells according to ABO blood group (matched - 1, mismatched - 1)
- CMVstatus - Serological compatibility of the donor and the recipient of hematopoietic stem cells according to cytomegalovirus
  infection prior to transplantation (the higher the value the lower the compatibility)
- RecipientCMV - Presence of cytomegalovirus infection in the donor of hematopoietic stem cells prior to transplantation (presence - 1, absence - 0)
- Disease - Type of disease (ALL,AML,chronic,nonmalignant,lymphoma)
- Riskgroup - High risk - 1, Low risk - 0,
- Txpostrelapse - The second bone marrow transplantation after relapse (No - 0; Yes - 1),
- Diseasegroup - Type of disease (malignant - 1, nonmalignant - 0), 
- HLAmatch - Compatibility of antigens of the main histocompatibility complex of the donor and the recipient of hematopoietic stem cells
$  according to ALL international BFM SCT 2008 criteria (10/10 - 0, 9/10 - 1, 8/10 - 2, 7/10 - 3 (allele/antigens)),
- HLAmismatch - HLA matched - 0, HL mismatched - 1,
- Antigen - In how many anigens there is difference beetwen the donor nad the recipient (-1 - no differences, 0 - one difference,1 (2) - two (three) diffences)
- Allel - In how many allele there is difference beetwen the donor nad the recipient {-1 no differences,0 - one difference, 1 (2) (3) - two, (tree, four) differences)
- HLAgrI - The differecne type beetwien the donor and the recipient (HLA mateched - 0,the difference is in only one antigen - 1,
  the difference is only in one allel - 2, the difference is only in DRB1 cell - 3, two differences (two allele or two antignes) - 4,
  two differences (two allele or two antignes) - 5),
- Recipientage - Age of the recipient of hematopoietic stem cells at the time of transplantation,
- Recipientage10 - Recipient age <10 - 0, Recipient age>=10 - 1,
- Recipientageint - Recipient age in (0,5] - 0, (5, 10] - 1, (10, 20] - 2,
- Relapse - Reoccurrence of the disease (No - 0, Yes - 1),
- aGvHDIIIIV - Development of acute graft versus host disease stage III or IV (Yes - 0, No - 1)
- extcGvHD - Development of extensive chronic graft versus host disease (Yes - 0, No - 1)
- CD34kgx10d6 - CD34+ cell dose per kg of recipient body weight (10^6/kg)
- CD3dCD34 - CD3+ cell to CD34+ cell ratio
- CD3dkgx10d8 - CD3+ cell dose per kg of recipient body weight (10^8/kg)
- Rbodymass - Body mass of the recipient of hematopoietic stem cells at the time of transplantation,
- ANCrecovery - Time to neutrophils recovery defined as neutrophils count >0.5 x 10^9/L 
- PLTrecovery - Time to platelet recovery defined as platelet count >50000/mm3,
- time_to_aGvHD_III_IV - Time to development of acute graft versus host disease stage III or IV
- survival_time numeric
- survival_status

**Data Sources:**

- [UCI Bone Marrow Transplant](https://archive.ics.uci.edu/dataset/565/bone+marrow+transplant+children)


## Project Goals
This initiative is designed to highlight the journey of implementing AI and machine learning models, including both existing ones and those that will be developed later on, with the goal of making them accessible to a wider community of users and developers.


#### Why build and use an machine learning pipeline?
In practical applications, it's essential to place models within a broader framework to unlock their potential for business. This process is known as deployment. Specifically in machine learning, deployment involves transitioning a model into a live production setting, allowing users or services to input data and receive predictions or insights from the model. This project aims to showcase the process of deploying AI and machine learning models, both those already developed and those that will be created in the future, making them available to a larger audience of users and developers. Additionally, it will illustrate how to streamline data preparation and the construction of machine learning models through automated pipelines, while also integrating these models into existing systems to leverage their advanced decision-making abilities.


## Data
A dataset that can be used to train the machine-learning model has been found. It is a CSV file containing 187 observations with 37 predictor variables and 1 target variable.  


## Conclusions
TBD...
***
## Technologies

- Python
- Jupyter Lab
- NumPy
- pandas
- Scipy
- sklearn
