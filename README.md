# Accenture Predictive Maintenance: Reducing Downtime Through Machine Learning
> **“Production Means Profit; Pumps Propel Product Through Pipes.”**

## Team Members


| Name | University | Contribution |
|------|-------------|---------------|
| **Sadhana Vasanthakumar** | Rutgers University | Led model definition and metric selection, co-developed baseline logistic regression, contributed to model evaluation and result interpretation. |
| **Krisha Patel** | Rutgers University | Authored project proposal, handled feature engineering, dealing with class imbalance and logistic regression modeling. |
| **Reeya Singh** | Rutgers University | Focused on feature engineering and model training across multiple model types. |
| **Mohnish Mehta** | Rutgers University | Supported model comparison and fine-tuning; contributed to hyperparameter optimization. |
| **Sophia Yan** | Rutgers University | Conducted exploratory data analysis and helped define early signal features (vibration, bearing temperature). |
| **Danniecia Gray** | Georgia State University | Managed GitHub setup, project documentation, business framing, and data cleaning; contributed to model evaluation and presentation design. |
| **Tony Christopher** | The City College of New York | Helped with data partitioning, training/test split (70:30), and logistic regression baseline testing. |
| **Aditi Manjunath** | Rutgers University | Assisted in data cleaning and model evaluation consistency checks. |

**AI Studio Coach:** Kaneesha Dawood  
**Challenge Advisor:** Kim Tennyson  


---

## Project Overview

Unplanned equipment downtime costs the oil and gas industry over **$40 billion** every year.  
Our project aims to change that through **predictive maintenance powered by machine learning**.

This project leverages synthetic sensor data from 50 industrial pumps to predict pump failures before they occur — giving maintenance teams the power to schedule repairs proactively, reduce downtime, and minimize operational losses.

### Project Goals
- Build a machine learning model that predicts pump failure likelihood.
- Help maintenance teams schedule repairs before breakdowns.
- Reduce downtime, extend equipment lifespan, and improve operational efficiency.

---

## Project Highlights

- Developed a predictive model using **classification-based machine learning** to forecast pump failures.  
- Identified **early-warning indicators** — notably **increased vibration** and **bearing temperature** — as strong predictors of failure.  
- Preprocessed over **720,000 time-series records** with no missing or duplicate values.  
- Achieved strong recall in detecting potential failures early, optimizing for reliability and operational impact.  
- Delivered actionable insights that can reduce unplanned downtime and improve cost efficiency in industrial maintenance systems.

---

## Setup and Installation

Follow these steps to reproduce and test the project:

1. **Clone the repository**
   ```bash
   git clone https://github.com/git@github.com:DannieciaGray/Accenture-2E-.git
   cd predictive-maintenance

2. **Create and activate a virtual environment**
    python -m venv venv
    source venv/bin/activate   # For Mac/Linux
    venv\Scripts\activate      # For Windows

3. **Install dependencies**
    pip install -r requirements.txt

4. **Run the notebook**
    Open and execute notebooks/predictive_maintenance.ipynb in Jupyter or VS Code.

5. **Access the dataset**
    The dataset is provided by AI Studio (synthetic data). It includes:

        Throughput

        Operating Pressure (bar)

        Vibration

        Bearing Temperature

        Pump Status (RUNNING vs DOWN)

## Data Understanding and Preparation 
Dataset size: 720,050 records from 50 pumps

Type: Synthetic time-series sensor data

Target: Pump Status (RUNNING vs DOWN)

Data quality: No duplicates, no missing values

Cleaning: Outliers handled via Winsorization

Feature engineering:

    -Normalization for comparability

    -Interaction terms between correlated features

    -Lag and rolling statistics for time-series modeling

    -Target definition: predict failure within the next X hours

## Modeling and Evaluation 
Our team explored several classification models, evaluating performance on accuracy, recall, and interpretability.

**Key Findings**
    Vibration and bearing temperature consistently rise before failures.

    The final model effectively detects early-stage faults.

    High recall ensured more true positives — essential in minimizing missed failures.

## Business Impact
Operational Continuity: Pumps are the heartbeat of refineries; our solution prevents production halts.

Financial Efficiency: Predictive insights reduce emergency repair costs and lost profit from downtime.

Process Optimization: Reliable pump performance ensures steady flow through pipelines — aligning with the 6 Ps:
Production Means Profit; Pumps Propel Product Through Pipes.

## Future Work 
    Integrate real-world IoT streaming data for live monitoring.
    Explore deep learning (LSTM or GRU) for improved temporal prediction.
    Develop a dashboard for real-time maintenance alerts.

## Acknowledgements
    Special thanks to:
        Break Through Tech AI for organizing the AI Studio Challenge
        Accenture for providing the industry problem statement
        Kaneesha Dawood and Kim Tennyson for their guidance and mentorship
