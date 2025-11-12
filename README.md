# 🎓 AI in Education — Evaluating Google Gemini 2.5 Flash on Physics Problems  

This project explores how **AI models like Google Gemini 2.5 Flash** perform when solving conceptual **physics questions**.  
It was done as part of an educational research-style assessment to test whether AI can understand reasoning-based academic problems and how prompt refinement affects its performance.

The main idea was to make Gemini act like a student answering real physics MCQs, analyze its accuracy, and see if adding hints or more context actually helps.

---

## 📘 Project Overview  

The work was divided into **four main tasks**, each targeting a different stage of evaluation:

### 🧩 Task 1 — Gemini Response and Evaluation  
- Loaded 25 multiple-choice physics questions (some had missing answers).  
- Used **Google Gemini 2.5 Flash API** with the free-tier key.  
- Sent each question (with options + images) to Gemini for reasoning-based answers.  
- Extracted Gemini’s chosen answer (A–D) and checked correctness manually.  
- Logged all results into an Excel sheet for review.

**Outcome:** Gemini achieved only **16% accuracy** overall. It struggled with deeper physics reasoning or multi-step problems, especially where image context was missing.

---

### 📊 Task 2 — Complexity Classification and Analysis  
- Added a **complexity classifier** (Easy / Medium / Hard) using keywords like *mirror*, *rotation*, *electric field*, etc.  
- Calculated Gemini’s accuracy by difficulty level.

**Findings:**

| Difficulty | Accuracy | Observation |
|-------------|-----------|-------------|
| Easy | 22% | Worked better for simple ray optics or formula-based questions. |
| Medium | 10% | Struggled with conceptual problems. |
| Hard | 17% | Random success, lacked proper logical chaining. |

**Insight:** The tougher the question, the lower Gemini’s reliability. It performs like a learner who remembers facts but fails at reasoning.

---

### 💡 Task 3 — Error Analysis and Prompt Refinement  
- Picked 5 wrong answers from Task 1 for re-evaluation.  
- Added **hints** to guide the model (like formula reminders or physical clues).  
- Compared responses before and after hinting.

**Observation:**  
After adding hints, Gemini gave longer and more structured reasoning, but correctness barely improved. It shows the model explains well, but doesn’t “think” like a human student.  
This experiment also highlighted that **prompt engineering improves clarity, not accuracy** for logic-heavy subjects.

📁 Final output: `physics_questions_final_with_hints.xlsx`

---

### 🧾 Task 4 — Role of AI in Education (Essay)  
In the essay, I discussed whether AI can democratize education and make learning accessible to everyone.

**Summary:**  
AI can surely make education global, but it needs open access, fairness, and local adaptation.  
Companies like **Google** can help by building **affordable AI tutors** that align with school curricula.  
As a **data enthusiast**, I believe my role is to help evaluate such models ethically and make sure they perform well across all learners.

---

## 🧰 Tools and Libraries Used  
- **Python** (Google Colab)  
- **Google Gemini API (GenAI)**  
- **Pandas**, **OpenPyXL**, **NumPy**, **Regex**, **Requests**  
- **Excel** for storing responses and evaluation  

---

AI-Education-Evaluation-Using-Gemini/
│
├── AI_Edu_Project_Code.ipynb                # Main Colab Notebook (Tasks 1–3)
├── physics_questions_with_gemini.xlsx       # Gemini responses and evaluation (Task 1)
├── physics_questions_with_complexity.xlsx   # Complexity classification results (Task 2)
├── physics_questions_final_with_hints.xlsx  # Refined prompt + hint evaluation (Task 3)
│
├── report.pdf                               # Final 5-page report combining all tasks
├── task4_essay.docx                         # Essay on “AI in Education” (Task 4)
│
├── README.md                                # Project overview and documentation
└── screenshots/                             # Output images from Colab runs
├── part1_output.png
├── part2_accuracy.png
├── part3_hints.png

## 📊 Key Takeaways  
- Gemini struggles with conceptual reasoning in physics.  
- Adding hints increases explanation quality, not accuracy.  
- Complex reasoning is still a big gap in current LLMs.  
- The project taught me how to evaluate AI performance systematically using real-world data.

---

## 🔗 Important Links  
**Google Colab Notebook:** [Open Here](https://colab.research.google.com/drive/16JkDIH6e6pCG25vYrVPxk4gz8ODMJyaf?usp=sharing)  
**Excel Outputs:** All `.xlsx` files are included in this repo.  
**Final Report:** Full summary of Tasks 1–4.

---

## 🧠 Reflection  
This was one of those projects that really taught me how to combine **AI reasoning with data analysis**.  
It showed how evaluating AI models scientifically can reveal their strengths and weaknesses in education.  
I learned not just coding or APIs, but how to think critically about model accuracy, reliability, and how data-driven evaluation shapes the future of learning.

---

## 📜 License  
This repository is open for **learning and portfolio purposes**.  
Feel free to explore or build on top of it.

---
