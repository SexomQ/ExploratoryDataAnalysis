# ExploratoryDataAnalysis

# European Development Indicators Analysis - Luxembourg

## Prerequisites

Before running this project, ensure you have the following installed:

- **Python 3.8 or higher**
- **pip** (Python package manager)
- **Jupyter Notebook** or **JupyterLab**

## Installation

### Step 1: Create a Virtual Environment inside the project folder

**On Windows:**
```bash
python -m venv .venv
.venv\Scripts\activate
```

**On macOS/Linux:**
```bash
python3 -m venv .venv
source .venv/bin/activate
```

### Step 2: Install Required Packages

```bash
pip install -r requirements.txt
```

## Project Structure

```
project-root/
│
├── EuropeanDevelopmentIndicatorsAcquisition.ipynb
├── requirements.txt
│
└── data_indicators/
    ├── ei_cphi_m_page_linear_2_0.csv
    ├── namq_10_gdp_page_linear_2_0.csv
    ├── nasa_10_nf_tr_page_linear_2_0.csv
    ├── une_rt_m_page_linear_2_0.csv
    ├── jvs_q_nace2_page_linear_2_0.csv
    ├── demo_pjangroup_page_linear_2_0.csv
    ├── migr_emi2_page_linear_2_0.csv
    ├── migr_imm8_page_linear_2_0.csv
    ├── demo_mlexpec_page_linear_2_0.csv
    ├── demo_gind_page_linear_2_0.csv
    ├── prc_hpi_q_page_linear_2_0.csv
    ├── namq_10_exi_page_export_linear_2_0.csv
    ├── namq_10_exi_page_import_linear_2_0.csv
    └── tipsbp40_page_linear_2_0.csv
```

## Data Requirements

### Create the Data Directory

```bash
mkdir data_indicators
```

### Required Data Files

Place the following 14 CSV files in the `data_indicators/` folder:

- `ei_cphi_m_page_linear_2_0.csv`
- `namq_10_gdp_page_linear_2_0.csv`
- `nasa_10_nf_tr_page_linear_2_0.csv`
- `une_rt_m_page_linear_2_0.csv`
- `jvs_q_nace2_page_linear_2_0.csv`
- `demo_pjangroup_page_linear_2_0.csv`
- `migr_emi2_page_linear_2_0.csv`
- `migr_imm8_page_linear_2_0.csv`
- `demo_mlexpec_page_linear_2_0.csv`
- `demo_gind_page_linear_2_0.csv`
- `prc_hpi_q_page_linear_2_0.csv`
- `namq_10_exi_page_export_linear_2_0.csv`
- `namq_10_exi_page_import_linear_2_0.csv`
- `tipsbp40_page_linear_2_0.csv`

## Running the Project

### Step 1: Activate Virtual Environment

**On Windows:**
```bash
.venv\Scripts\activate
```

**On macOS/Linux:**
```bash
source .venv/bin/activate
```

### Step 2: Launch Jupyter Notebook

```bash
jupyter notebook
```

### Step 3: Run the Notebook

1. Click on `EuropeanDevelopmentIndicatorsAcquisition.ipynb`
2. Click `Kernel` → `Restart & Run All`

## Troubleshooting

### Common Issues

**Issue: ModuleNotFoundError**
```
Error: ModuleNotFoundError: No module named 'pandas'
```
**Solution**: Activate virtual environment and install requirements:
```bash
pip install -r requirements.txt
```

**Issue: FileNotFoundError for Data Files**
```
Error: FileNotFoundError: data_indicators/ei_cphi_m_page_linear_2_0.csv
```
**Solution**: 
- Create the `data_indicators/` folder
- Add all 14 required CSV files
- Check filenames match exactly (case-sensitive)

**Issue: Jupyter Kernel Not Found**
```
Error: No kernel found
```
**Solution**: Install IPython kernel:
```bash
python -m ipykernel install --user --name=.venv
```