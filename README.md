# 🤖 Which AI Skills Are Most Valuable in the Job Market?

## 📌 Overview
This project explores the value of AI-related skills in the job market by combining job posting data with online discussion trends. The goal is to identify which AI skills are associated with higher salaries, which locations pay more for specific AI roles, and whether the most discussed skills online are also the most financially rewarding.

## 🎯 Objectives
We investigate the following key questions:

- Which AI skills are associated with higher salaries?  
- Which company locations pay more for specific AI roles?  
- Are the most discussed AI skills online also the highest paid?  
- Which skills appear to be undervalued or overhyped?  

## 📊 Dataset
- Source: Kaggle — *Global AI Job Market and Salary Trends 2025*  
- Format: CSV  
- Key variables: `job_title`, `salary_usd`, `salary_currency`, `company_location`, `required_skills`  

We also use the **Stack Exchange API** to measure discussion volume for AI-related skills over the past 3 months.

## ⚙️ Tools Used
- Python (Pandas, Requests)  
- Jupyter Notebook / Google Colab  
- Matplotlib  
- Stack Exchange API  

## 🧹 Data Cleaning
We applied several preprocessing steps to prepare the data:
- Handling missing salary and skill values  
- Standardizing salary values into USD  
- Splitting and cleaning the `required_skills` column  
- Transforming multi-skill rows into one row per skill  
- Filtering skills into AI-specific and supporting categories  

## 🤖 AI-Specific Skills
For this project, the following skills were treated as **AI-specific**:

- NLP  
- Deep Learning  
- MLOps  
- Computer Vision  
- PyTorch  
- TensorFlow  

All other listed skills in the dataset were treated as supporting technical skills.

## 📈 Key Insights

### 💰 Salaries by Skill
- AI-related job postings include both AI-specific and supporting technical skills  
- Median salary was used as the main salary metric to reduce the effect of outliers  
- Skills were compared based on how strongly they were associated with higher-paying roles  

### 🌍 Locations and Roles
- Salaries were compared by `company_location` and `job_title`  
- Since the dataset does not include a dedicated `country` column, `company_location` was used as the closest location field  
- This helped identify which locations pay more for specific AI roles  

### 💬 Online Discussion vs Salary
- Stack Overflow discussion volume was used as a proxy for online attention  
- Question counts over the last 3 months were compared against salary rankings  
- This allowed us to see whether the most discussed AI skills are also the highest paid  

### 📉 Overhyped vs Undervalued Skills
- **Overhyped**: skills discussed more than their salary ranking suggests  
- **Undervalued**: skills paid more than their discussion ranking suggests  
- **Aligned**: skills whose discussion and salary rankings are similar  

## 🧪 Workflow
1. Data exploration and question definition  
2. Data cleaning and salary standardization  
3. Skill extraction and classification  
4. Salary analysis by skill  
5. Salary analysis by role and location  
6. Stack Exchange API analysis for discussion trends  
7. Comparison of salary rank and discussion rank  
8. Insights and interpretation  

## 👥 Team Approach
- Data preparation and cleaning  
- Salary analysis and visualizations  
- API-based discussion analysis  
- Insight generation and final presentation  

## 🚀 Deliverables
- Jupyter Notebook    
- Cleaned dataset  
- Visualizations  
- README  
- Final presentation  

## 📌 Conclusion
This project compares job-market value and online discussion attention for AI-related skills. It shows that skills discussed more frequently online are not always the highest paid, and that some skills may receive less attention despite being associated with strong salaries. These results provide a more balanced view of which AI skills are most valuable in practice.

## 🔗 Links
- Dataset: https://www.kaggle.com/datasets/bismasajjad/global-ai-job-market-and-salary-trends-2025  
- Stack Exchange API: https://api.stackexchange.com/docs  
- Repository: https://github.com/baharmnb/BANDANA-Project  
- Presentation: https://prezi.com/p/edit/kumbk8uqqly_/  
