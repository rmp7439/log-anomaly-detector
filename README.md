# Log Anomaly Detector

Hybrid anomaly detection system for identifying suspicious activity in Linux authentication logs using rule-based analysis and Isolation Forest.

## Features

- Parse Linux authentication logs into structured datasets
- Detect common attack patterns with rule-based analysis
- Identify statistical anomalies using Isolation Forest
- Combine both approaches for improved detection coverage
- Generate severity-ranked security alerts
- Visualize anomaly trends and feature distributions

## Tech Stack

- Python
- pandas
- NumPy
- scikit-learn
- Matplotlib

## Getting Started

```bash
git clone https://github.com/rmp7439/log-anomaly-detector
cd log-anomaly-detector
pip install -r requirements.txt
jupyter lab detector.ipynb
```

## Project Structure

```text
log-anomaly-detector/
├── detector.ipynb
├── results/
├── requirements.txt
├── .gitignore
└── README.md
```

## Results

### Detection Results

| Detector | Alerts |
|-----------|-------:|
| Rule Engine | 44 |
| Isolation Forest | 13 |
| Hybrid | 53 |

### Severity Breakdown

| Severity | Count |
|----------|------:|
| HIGH | 4 |
| MEDIUM | 40 |
| LOW | 9 |

### Anomaly Timeline

![Anomaly Timeline](results/anomaly_timeline.png)

### Feature Distribution

![Feature Distribution](results/feature_distribution.png)

## Future Improvements

- Streamlit dashboard for interactive monitoring
- Sequence-based anomaly detection with LSTM Autoencoders
- Support for additional log formats
- Email and Slack alerting for high-severity events
