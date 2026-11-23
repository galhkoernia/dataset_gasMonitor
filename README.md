# MQ-2 Telemetry Analysis

A Python-based data analysis project for processing and visualizing telemetry collected from an ESP32-based MQ-2 gas detection prototype.

The project focuses on inspecting raw telemetry data, performing basic data cleaning, exploring sensor behavior, and generating visualizations as preparation for further data analysis and potential machine learning development.

## Features

- Raw telemetry data inspection
- Missing-value and duplicate detection
- Timestamp and numerical data conversion
- Basic data cleaning
- Exploratory data analysis
- MQ-2 sensor value visualization
- Gas detection status visualization
- Sensor transition analysis
- Cleaned dataset generation

## Project Structure

```text
assets/
├── gas_monitor.csv
├── gas_monitor_clean.csv
└── mq2_telemetry_analysis.ipynb
```

### Dataset

`gas_monitor.csv` contains telemetry data collected from the MQ-2 gas detection prototype.

The dataset includes information such as:

- `device_id`
- `sensor`
- `value`
- `gas_status`
- `timestamp`

The cleaned dataset is exported as:

```text
gas_monitor_clean.csv
```

## Analysis Workflow

The notebook follows a structured data analysis workflow:

```text
Raw Telemetry
      ↓
Data Inspection
      ↓
Data Cleaning
      ↓
Exploratory Data Analysis
      ↓
Data Visualization
      ↓
Sensor Behavior Analysis
      ↓
Clean Dataset
      ↓
Further Analysis / Machine Learning
```

Machine learning is not applied as part of the initial analysis. The dataset is first evaluated to determine whether the available telemetry contains sufficient information for a meaningful machine learning task.

## Technologies

- Python
- Jupyter Notebook
- Pandas
- Matplotlib

## Environment Setup

Create a virtual environment:

```bash
python -m venv .venv
```

Activate the environment on Windows:

```bash
.venv\Scripts\activate
```

Install the required dependencies:

```bash
pip install pandas matplotlib jupyter
```

Run Jupyter Notebook:

```bash
jupyter notebook
```

Alternatively, the notebook can be opened directly through Visual Studio Code using the Jupyter extension.

## Analysis Notebook

The main analysis is contained in:

```text
mq2_telemetry_analysis.ipynb
```

The notebook is organized into several stages:

1. Import libraries
2. Load telemetry dataset
3. Inspect dataset structure
4. Check missing and duplicated records
5. Clean telemetry data
6. Explore sensor and gas-status distributions
7. Visualize sensor behavior over time
8. Analyze sensor value transitions
9. Export the cleaned dataset

## Future Development

Possible extensions include:

- Moving average filtering
- Sensor response analysis
- Noise and outlier analysis
- Feature engineering
- Analog MQ-2 data analysis
- Machine learning classification
- Model evaluation and visualization

These extensions will be implemented only after the characteristics and quality of the telemetry data have been properly evaluated.

## Developed by

**Galuh Kurnia Pratama**

Physics student focused on embedded systems, instrumentation, software engineering, and technical research.