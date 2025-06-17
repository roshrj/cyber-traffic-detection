# Cybersecurity Web Traffic Detection

This project analyzes web server traffic data to detect suspicious activity using machine learning and anomaly detection techniques.

## Dataset Overview

Each record in the dataset represents a traffic stream and includes:

* `bytes_in`, `bytes_out`, `session_duration`, `bytes_ratio`, `hour`
* `protocol`, `src_ip_country_code`, `rule_names`, `time`
* `response.code`, `src_ip`, `dst_ip`, and other metadata

## Project Structure

This project is divided into three main modules:

### Module 1: Security Analysis (EDA)

* Count plots of suspicious vs. normal traffic by protocol
* Top 10 countries with suspicious activity
* Session duration distribution of suspicious traffic

### Module 2: Classification (Random Forest)

* Features selected: bytes, duration, protocol, country code, etc.
* Label: `is_suspicious` (based on presence of rule name)
* Metrics: Classification report, confusion matrix

### Module 3: Anomaly Detection (Isolation Forest)

* Unsupervised detection of anomalous traffic patterns
* Visualization using PCA
* Output: `is_anomaly` column

## Visualizations

* Suspicious traffic by protocol and by country
* PCA-based scatterplot of anomalies
* Time-based trend of suspicious events

## 📃 Files

* Web Traffic suspicious threats.ipynb: Main notebook
* CloudWatch_Traffic_Web_Attack.csv`: Output dataset with predictions

## ⚖️ Tech Stack

* Python
* pandas, matplotlib, seaborn
* scikit-learn

## ⚡ How to Use

1. Clone the repository
2. Add the dataset as `cybersecurity_web_traffic.csv`
3. Run `Cyber_Traffic_Detection.ipynb`
4. View plots and predictions

## 📈 Output Example

```
Anomalies Detected: 3
```

## 👤 Author

Aspiring Data Scientist | Project by Roshine Jose


