# Employee Sentiment Analysis 📖

This project analyzes a dataset of employee emails to assess sentiment and engagement. Using Natural Language Processing (NLP) in Python, the analysis labels employee messages, calculates monthly sentiment scores, identifies potential flight risks, and provides actionable insights into the overall morale within the organization.

---

## Setup and Installation ⚙️

Follow these steps to set up the project environment and run the analysis.

### 1. Prerequisites
- Python 3.8+
- pip (Python package installer)

### 2. Create the Environment
First, clone the repository and navigate into the project directory. Then, it's recommended to create and activate a virtual environment.

```bash
# Clone the repository (replace with your actual repo link)
git clone [https://github.com/your-username/Employee-Sentiment-Analysis.git](https://github.com/your-username/Employee-Sentiment-Analysis.git)

# Create and activate a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

### 3. Install Dependencies
This project requires a few key Python libraries. Create a file named **`requirements.txt`** in your project folder with the content below.

**`requirements.txt`:**
```
pandas
matplotlib
seaborn
scikit-learn
```
Now, run the following command in your terminal to install them all at once:
```bash
pip install -r requirements.txt
```

### 4. Run the Analysis
All the code for this project is contained in a single Jupyter Notebook. Launch Jupyter and open the file to see the entire process.

```bash
jupyter notebook employee_sentiment_analysis.ipynb
```

---

## Project Summary & Key Findings 📊

### Top Three Positive Employees
Based on the highest monthly sentiment scores, these employees consistently demonstrated positive communication.
- **sally.beck@enron.com**
- **john.arnold@enron.com**
- **patti.thompson@enron.com**

### Top Three Negative Employees
Based on the lowest (most negative) monthly sentiment scores, these employees showed the most negative communication.
- **eric.bass@enron.com**
- **don.baughman@enron.com**
- **kayne.coulter@enron.com**

### List of Employees Flagged as Flight Risks
An employee is flagged as a flight risk if they sent **4 or more negative emails in a rolling 30-day period**. The analysis identified the following employees:
- **eric.bass@enron.com**
- **rhonda.denton@enron.com**

### Key Insights and Recommendations
* **Insight 1: Overall Sentiment is Healthy.** The majority of communications are neutral or positive, which is expected in a professional setting. There is no evidence of widespread negative morale.
* **Insight 2: Negativity is Concentrated.** Negative sentiment is not widespread but is concentrated among a few specific individuals. This suggests that any issues may be localized rather than systemic.
* **Recommendation:** It is recommended that HR or management review the individuals identified in the **"Top Negative"** and **"Flight Risk"** categories. A supportive check-in could help identify and address potential root causes like high stress, workload, or interpersonal conflicts, ultimately improving employee retention.