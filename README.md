Healthcare Diagnostic and Treatment
Objective
Healthcare Diagnostic and Treatment is designed to help users identify potential diseases based on their symptoms, providing basic treatment advice, lifestyle tips, and urgency levels for medical attention. It also logs user feedback for future improvements.
Disclaimer: This tool is not a substitute for professional medical advice. Always consult a doctor before taking any medication.
Features
•  Diagnoses 7 common diseases based on user-input symptoms (e.g., fever, chest pain, sore throat).
•  Provides treatment advice, including medicines and lifestyle recommendations.
•  Assigns urgency levels (low, medium, high) to guide users on seeking medical attention.
•  Logs user feedback with timestamps in a feedback.log file for analysis.
•  Includes a disclaimer to ensure users consult a doctor for professional advice.
Technology Used
•  Language: Python
•  Libraries:
	•  datetime for timestamp logging.
•  Tools:
	•  File I/O for saving feedback to feedback.log.
How It Works
1.  The user enters their name and a brief description of their symptoms (e.g., “I have a fever”).
2.  The program uses a smart_match function to match the input symptoms to a predefined database of 7 diseases.
3.  If a match is found, it outputs:
	•  The possible disease.
	•  Urgency level (low, medium, or high).
	•  Treatment advice, including medicines and lifestyle tips.
	•  A note about the condition.
4.  The user is asked for feedback (“Was this helpful?”), which is logged with a timestamp.
5.  The program loops until the user chooses to exit by typing “exit”.
Data Collection
•  The dataset is a hardcoded dictionary (disease_db) in the Python script.
•  It contains 7 diseases (e.g., Viral Infection, Gastritis, Angina) with their symptoms, treatments, and urgency levels.
•  No external data sources were used; the dataset was manually curated for this project.
