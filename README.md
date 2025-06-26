# Paroxysmal Nocturnal Haemoglobinuria (PNH) Diagnosis & Early Detection Model

PNH is a very rare condition that can be difficult to diagnosis due to non-specific presentation and lack of specific workup.  We have built and are providing a machine learning algorithm that can be used to identify patients who may warrant appropriate workup for PNH.

Key definitions:
- Applicable population:  Patients having a hemoglobin (Hb) laboratory draw (typically part of a complete blood count (CBC) panel
- Target for prediction: ICD-10 for PNH (D59.5) within 3 to 12 months of the Hb draw
- Key features:
  <ol type="1">
     <li>Aplastic anemia in the prior 24 months</li>
     <li>Charlson comorbidity index (continous integer)</li>
     <li>Aplastic anemia in the prior 12 months (coded 0/1)</li>
     <li>Age (continuous)</li>
     <li>Anemia broad in the prior 6 months (coded 0/1)</li>
     <li>Low haptoglobin in the prior 24 months (coded 0/1)</li>
     <li>Myelodysplastic syndrome diagnosis in the primary 3 months (coded 0/1)</li>
     <li>Most recent creatinine lab value within 24 months (continuous)</li>
     <li>Race (categories: )</li>
     <li>Ethnicity (values: )</li>
     <li>Most recent hemoglobin lab value in the prior 6 months</li>
     <li>Most recent lactate dehydrogenase (LDH) lab value in the prior 6 months</li>
  </ol>

Key technical requirements:
- XGBoost:  The best performing model was XGBoost (https://xgboost.readthedocs.io/en/stable/).  A portable XGBoost model is provided and can be utilized with the XGBoost package in languages such as Python or R.

General notes about performance:
- 

General notes about methods:
- The model was trained using electronic health record (EHR) data covering 67MM patients in the United States
- Limited 
