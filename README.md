# Resume Shortlisting
This AI-powered project automates resume shortlisting by scoring resumes based on experience, skills, and education. It extracts experience using advanced regex, matches job description keywords, and supports formats like PDF. Optimized for fast processing, it streamlines recruitment by highlighting the top 5 candidates.

## Resume Shortlisting Automation with AI

This project is designed to automate the process of resume shortlisting by using AI-driven methods to evaluate and score resumes based on relevant experience, skills, and educational qualifications. It aims to streamline the recruitment process, making it more efficient and accurate by highlighting the most suitable candidates for a job description.

### Key Features

- **Experience Extraction**: 
  - The system employs advanced regular expressions (regex) to extract and calculate years of experience from various formats. It handles explicit experience mentions like "10+ years", and date ranges such as "2020 May to 2023 Aug," converting these into a numerical value contributing to the overall resume score.
  
- **Keyword Matching**:
  - The system efficiently matches keywords from job descriptions to the content of resumes. It identifies and scores relevant skills, certifications, and educational qualifications, prioritising candidates with the most appropriate backgrounds.
  
- **Scoring System**:
  - The resume scoring system is designed to be flexible and comprehensive. It assigns scores based on years of experience, relevant skills, and educational qualifications. This scoring system can be customized to fit the specific needs of different job roles or industries.
  
- **Batch Processing**:
  - The tool is optimized to process large resumes quickly and efficiently. This is particularly useful for large-scale recruitment drives where hundreds or thousands of resumes must be screened quickly.
  
- **Streamlined Recruitment**:
  - By automating the candidate evaluation process, this project significantly reduces the time and effort required for manual resume screening. It ensures that only the most qualified individuals are highlighted for further consideration, making the recruitment process more effective.

### Installation and Setup

1. **Clone the Repository**:  
   ```
   git clone https://github.com/Jasl-hub/resume-shortlisting-ai.git
   
   ```

2. **Install Dependencies**:  

   ```
   pip install -r requirements.txt
   ```

3. **Run the Script**:  
   You can start processing resumes by running the main script:
   ```
   python resume_shortlisting.py
   ```

4. **Configure Scoring System**:  
   Customize the scoring system by modifying the `data_map` in the script, where you can set the weight for different experience ranges, skills, and educational qualifications.

### Usage

- **Dataset**: Provide resumes in PDF format. The dataset has been taken from: https://www.kaggle.com/datasets/sauravsolanki/hire-a-perfect-machine-learning-engineer
- **Output**: The system will generate a list of 5 candidates with scores, highlighting those who best match the job requirements.

### Customization

- **Regex Customization**: The regex patterns used for extracting years of experience and other qualifications can be modified to suit specific requirements or different formats that might be encountered.
  
- **Keyword Dictionary**: The system uses a keyword dictionary that can be updated to include industry-specific terms, certifications, and skills.

### Contributing

Contributions to improve the project are welcome! Please fork the repository, create a new branch, and submit a pull request.

---
