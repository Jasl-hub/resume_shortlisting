# 🤖 Resume Shortlisting using AI & Keyword Matching

This project automates the resume shortlisting process by extracting keywords from job descriptions, parsing resumes, calculating years of experience, and scoring resumes based on relevance. It is designed to assist recruiters in filtering the most suitable candidates efficiently.

---

## 📁 Project Structure

```
resume_shortlisting/
├── 1_resume_shortlist_wo_ML.py                       # Rule-based resume shortlisting using keyword matching
├── 2_resumeparsing_without_bert_(spacy_+_tf_idf).py  # Resume parsing and scoring using SpaCy and TF-IDF
├── 3_bert_resume_shortlisting_complete.py            # Resume shortlisting using BERT embeddings
├── 4_unified_evaluation_framework_bert_&_tfidf_&_hybrid.py  # Unified scoring and comparison framework for BERT, TF-IDF, and Hybrid models
├── tfidf_vs_bert.png                                 # Visualization comparing TF-IDF vs BERT performance
├── tfidf_vs_bert_vs_hybrid.png                       # Visualization comparing all three approaches
├── HIREAIML_sample.zip                               # Sample input data (job descriptions and resumes)
├── requirements.txt                                  # Python dependencies
├── README.md                                         # Project overview and instructions
```



---

## 🚀 Features

- 🔍 Keyword Extraction from job descriptions (skills, education, certifications, experience)
- 📄 Resume Parsing for PDFs using PyPDF2
- ⏳ Experience Calculation from natural language and date ranges
- 🧠 Resume Scoring based on:
  - Matched skills
  - Educational qualifications
  - Calculated years of experience
- 🏆 Final Shortlist Generation with visual score summary

---

## 🛠️ How to Use

### 1. Clone the repository

```bash
git clone https://github.com/Jasl-hub/resume_shortlisting.git
cd resume_shortlisting
```

### 2. Install the required packages

```bash
pip install -r requirements.txt
```

### 3. Prepare your input data

- Place **Job Description files** in a folder named `job_descriptions/`
- Place **Resumes (PDF format)** in a folder named `resumes/`

### 4. 🧠 Approach Overview
This project follows a step-by-step evolution from simple rule-based logic to advanced ML-based resume shortlisting methods:

🔹 a. Rule-Based Shortlisting (No ML)
File: 1_resume_shortlist_wo_ML.py

Matches resumes with job descriptions using extracted keywords (skills, education, experience).

Simple, fast, and interpretable.

Limitation: Cannot understand context or synonyms.

🔹 b. TF-IDF + SpaCy Matching
File: 2_resumeparsing_without_bert_(spacy_+_tf_idf).py

Uses TF-IDF and cosine similarity to rank resumes based on keyword importance.

Better than raw keyword matching.

Limitation: Still lacks deep semantic understanding.

🔹 c. BERT-Based Shortlisting
File: 3_bert_resume_shortlisting_complete.py

Leverages BERT embeddings to compare resumes and JDs semantically.

Captures context and meaning, even when wording differs.

Limitation: Slower and resource-intensive.

🔹 d. Unified Evaluation Framework (TF-IDF + BERT + Hybrid)
File: 4_unified_evaluation_framework_bert_&_tfidf_&_hybrid.py
Visuals: tfidf_vs_bert.png, tfidf_vs_bert_vs_hybrid.png

Compares all three methods and introduces a hybrid approach.

Balances performance and accuracy.

Useful for adapting to different hiring needs.

✅ Use rule-based for quick filtering, TF-IDF for a balance, and BERT/hybrid for precision matching.



---

## 📊 Output

The script will generate a file called `tfidf_vs_bert_vs_hybrid.png` or `tfidf_vs_bert.png`, displaying the shortlisted candidates along with their scores.

---

## 📌 Future Improvements

- 🖥 Add GUI or Streamlit-based interface
- 📘 Include support for DOCX resumes and multilingual documents
- 🚀 Deploy the entire pipeline as a web application using Streamlit or Flask for easy recruiter interaction and resume upload.

---

## 📄 License

This project is open-sourced under the **MIT License**.

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome!  
Feel free to open issues or submit pull requests.
