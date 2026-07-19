## 🗂 Dataset

**Dataset:** Impact of AI on Students
**Source:** [Kaggle — laveshjadon/ai-impact-on-students](https://www.kaggle.com/datasets/laveshjadon/ai-impact-on-students)
**Size:** 50,000 rows × 16 columns
**Key features:** Weekly GenAI Hours, Traditional Study Hours, Prompt Engineering
Skill, Institutional Policy, Burnout Risk Level, Skill Retention Score, Pre/Post GPA

## 🔍 Key Findings

- **GPA change** showed no meaningful correlation with weekly AI usage hours —
  more AI use does not predict better or worse grades
- **Skill retention** was positively associated with traditional study hours and
  tool diversity
- **Burnout risk** classification achieved only ~52% accuracy across all models
  (Logistic Regression, Random Forest), barely above the majority class baseline.
  Feature importance analysis revealed that `Weekly_GenAI_Hours` drove 90% of
  predictions yet still could not separate burnout levels — strongly suggesting
  that `Burnout_Risk_Level` was assigned independently of other features in this
  synthetic dataset
- This highlights an important real-world lesson: model performance must always
  be interpreted in the context of data quality

## ⚙️ How to Run

```bash
git clone https://github.com/OlgaNazarenko/ai-impact-on-students.git
cd ai-impact-on-students
pip install -r requirements.txt
```

Then open the notebooks in order starting with `01_eda/`.

## 🛠 Tools & Libraries

Python, pandas, NumPy, scikit-learn, matplotlib, seaborn, scipy