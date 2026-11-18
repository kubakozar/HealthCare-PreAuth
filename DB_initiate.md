# Initial prompt

Generate create table command for creating clinical_history table,
also, take below record as a sample and generate 5-6 sql insert
statements for astradb clinical_history table: patient_id = 10026
clinical_history = Patient diagnosed with hypothyroidism. Symptoms
include fatigue and weight fluctuations. Lab results confirmed low
thyroid levels. Started on levothyroxine therapy. patient_name=Ananya
Das last_visit_date=2026-02-05 age=33

# Results

CREATE TABLE default_keyspace.clinical_history (
patient_id INT PRIMARY KEY,
patient_name TEXT,
age INT,
last_visit_date DATE,
clinical_history TEXT
);

INSERT INTO default_keyspace.clinical_history (patient_id,
patient_name, age, last_visit_date, clinical_history)
VALUES (10026, 'Ananya Das', 33, '2026-02-05', 'Patient diagnosed with
hypothyroidism. Symptoms include fatigue and weight fluctuations. Lab
results confirmed low thyroid levels. Started on levothyroxine
therapy.');

INSERT INTO default_keyspace.clinical_history (patient_id,
patient_name, age, last_visit_date, clinical_history)
VALUES (10027, 'Rajesh Kumar', 45, '2026-03-12', 'Patient diagnosed
with Type 2 Diabetes Mellitus. Presenting symptoms include increased
thirst, frequent urination, and blurred vision. HbA1c level at 8.2%.
Prescribed metformin 500mg twice daily and dietary modifications.');

INSERT INTO default_keyspace.clinical_history (patient_id,
patient_name, age, last_visit_date, clinical_history)
VALUES (10028, 'Priya Sharma', 52, '2026-01-28', 'Patient presents
with essential hypertension. Blood pressure readings consistently
above 140/90 mmHg. No significant family history. Started on
amlodipine 5mg daily and advised lifestyle modifications including
low-sodium diet and regular exercise.');

INSERT INTO default_keyspace.clinical_history (patient_id,
patient_name, age, last_visit_date, clinical_history)
VALUES (10029, 'Mohammed Ali', 28, '2026-04-15', 'Patient with history
of bronchial asthma since childhood. Recent exacerbation with wheezing
and shortness of breath. Spirometry shows moderate obstruction.
Prescribed inhaled corticosteroids and salbutamol inhaler for rescue
therapy.');

INSERT INTO default_keyspace.clinical_history (patient_id,
patient_name, age, last_visit_date, clinical_history)
VALUES (10030, 'Sneha Patel', 38, '2026-02-20', 'Patient complains of
chronic fatigue, muscle weakness, and bone pain. Laboratory tests
reveal severe Vitamin D deficiency with levels at 12 ng/mL. Started on
Vitamin D3 supplementation 60,000 IU weekly for 8 weeks, followed by
maintenance dose.');

INSERT INTO default_keyspace.clinical_history (patient_id,
patient_name, age, last_visit_date, clinical_history)
VALUES (10031, 'Amit Verma', 41, '2026-03-08', 'Patient diagnosed with
GERD. Symptoms include persistent heartburn, regurgitation, and
difficulty swallowing. Endoscopy revealed mild esophagitis. Prescribed
proton pump inhibitor omeprazole 20mg before breakfast and advised
dietary changes to avoid trigger foods.');