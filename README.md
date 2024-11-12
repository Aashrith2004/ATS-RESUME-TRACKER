# ATS-RESUME-TRACKER


### Overview:
CareerCraft leverages advanced ATS (Applicant Tracking System) technology to help job seekers optimize their resumes for job applications. It analyzes resumes against job descriptions, offering personalized feedback and suggestions to improve alignment with the job roles.

### Key Features:
- **ATS-Optimized Resume Analysis**: Analyzes how well your resume matches a provided job description (JD).
- **Resume Optimization**: Suggests improvements to enhance your resume's effectiveness.
- **Skill Enhancement**: Identifies missing keywords and skills.
- **Career Progression Guidance**: Helps navigate career growth based on resume performance.
- **Tailored Profile Summaries**: Provides personalized summaries for your resume based on the JD.
- **Streamlined Application Process**: Simplifies the process of tailoring resumes to specific job roles.
- **Personalized Recommendations**: Offers customized advice based on your resume and JD.
- **Efficient Career Navigation**: Helps guide users in optimizing their resumes for various career paths.

### Workflow:
1. **Job Description and Resume Upload**: Users paste the job description and upload their resume (PDF format).
2. **Resume Analysis**: The system processes the resume using `PyPDF2` to extract text, and uses **Google Gemini** to analyze the content and provide insights.
3. **ATS Match Calculation**: The tool calculates how well the resume matches the job description, identifying missing keywords and offering a summary of the user’s qualifications.
4. **Response Display**: The results are shown in a structured format:
   - Percentage match with JD.
   - List of missing keywords.
   - Profile summary based on the JD.

### UI:
- Streamlit provides a web interface with interactive elements like text areas and file uploaders.
- Various sections offer visual explanations and services, such as offerings and FAQs.
- The layout is well-structured, with distinct areas for the resume upload, job description input, and results display.

This application can help job seekers tailor their resumes, improve job application success, and navigate their career paths more effectively.
