# 📊 Vanguard A/B Test — Digital Experience Redesign  
### Customer Experience (CX) — Data Analysis Project

## 🧩 Overview  
This project analyzes Vanguard’s digital redesign experiment, where a new modern UI with in‑context prompts was tested against the traditional interface.  
The main question: **Did the new UI increase completion rates and improve user experience?**

The A/B test ran from **15 March 2017 to 20 June 2017**, comparing:

- **Control Group:** traditional interface  
- **Test Group:** redesigned interface with modern UI + contextual prompts  

Both groups followed the same online process: initial page → 3 steps → confirmation.

---

## 🔗 Project Links  
- **GitHub Repository:** https://github.com/mocihu-source/Week-5-6-EDA-and-Inferential-Stats  
- **Trello Kanban Board:** https://trello.com/b/6a550d61be8094511b4f3f2b  
- **Jupyter Notebook (Online):** https://jupyter.org/try-jupyter/lab/index.html  
- **Tableau Public:** *(link to be added when published)*  

---

## 📁 Project Structure  

---

## 📚 Datasets  

### **1. Client Profiles — `df_final_demo`**  
Demographics & account info:  
- `client_id`, `clnt_age`, `gendr`, `num_accts`, `bal`  
- `clnt_tenure_yr`, `clnt_tenure_mnth`  
- `calls_6_mnth`, `logons_6_mnth`

### **2. Digital Footprints — `df_final_web_data_pt_1` + `pt_2`**  
Merged to form full user navigation logs:  
- `visitor_id`, `visit_id`, `process_step`, `date_time`

### **3. Experiment Roster — `df_final_experiment_clients`**  
Shows group assignment:  
- `client_id`, `variation` (Test vs Control)

---

## 🔍 Tasks & Methodology  

### **Week 5 — Day 1 & 2: EDA & Cleaning**
- Merge web data  
- Handle missing values & duplicates  
- Explore demographics  
- Analyze navigation patterns  

### **Week 5 — Day 3: Performance Metrics**
KPIs implemented:
- **Completion Rate**  
- **Time Spent per Step**  
- **Error Rate (backward navigation)**  

### **Week 5 — Day 4 & 5: Hypothesis Testing**
Tests performed:
- **Two‑proportion z‑test** (completion rate difference)  
- **One‑sided z‑test** (cost‑effectiveness threshold: +5%)  
- Additional optional tests  

### **Week 6 — Day 1 & 2: Tableau**
Interactive dashboard with:
- Completion rates  
- Step durations  
- Error rates  
- Demographic filters  

### **Week 6 — Day 3 & 4: Finalization**
- Code organization  
- README polishing  
- Slide preparation  
- Optional bonus tasks (power analysis, Streamlit prototype)

---

## 📈 Key Metrics  

### **Completion Rate**


\[
\text{Completion Rate} = \frac{\text{Users reaching 'confirm'}}{\text{Total users in group}}
\]



### **Time Spent per Step**
Average duration between consecutive steps.

### **Error Rate**


\[
\text{Error Rate} = \frac{\text{Backward steps}}{\text{Total steps}}
\]



---

## 🧪 Hypothesis Tests  

### **Completion Rate Difference**
- **H₀:** Test = Control  
- **Hₐ:** Test ≠ Control  
→ Two‑proportion z‑test

### **Cost‑Effectiveness Threshold (+5%)**
- **H₀:** Test ≤ Control + 5%  
- **Hₐ:** Test > Control + 5%  
→ One‑sided z‑test

---

## 🧪 Experiment Evaluation  
Topics covered:
- Randomization quality  
- Duration adequacy (3 months)  
- Potential biases  
- Missing data considerations  
- Additional data needs (e.g., device type, error logs, page load times)

---

## 📊 Tableau Dashboard  
Includes:
- Completion rate comparison  
- Step duration heatmaps  
- Error rate charts  
- Filters for age, gender, tenure, account balance  

---

## 🛠️ Tech Stack  
- Python (Pandas, NumPy, SciPy, Matplotlib, Seaborn)  
- Jupyter Notebook  
- Tableau  
- Streamlit (optional)  
- GitHub + Trello (Kanban board)

---

## 🎯 Deliverables  
✔ GitHub repository  
✔ Jupyter notebook  
✔ `.py` modules  
✔ Tableau dashboard  
✔ Slides link  
✔ README (this file)  
✔ Trello board link  
✔ Clean, organized codebase  

---

## 🗣️ Presentation Structure  
- Title & introduction  
- Data overview  
- EDA  
- KPIs  
- Hypothesis testing  
- Experiment evaluation  
- Tableau demo  
- Teamwork  
- Challenges & learnings  
- Conclusion & recommendations  

---

## 📌 Author  
**Teresa Mendes Coelho**  
Data Analyst — Vanguard CX Case Study

