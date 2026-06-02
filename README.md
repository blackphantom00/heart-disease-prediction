
## Create a Virtual Environment

### Linux / macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Generate Data and Train Models

```bash
python data/generate_data.py
python notebooks/heart_disease_analysis.py
```

## Run the Application

```bash
streamlit run app/app.py
```

## Open in Browser

```text
http://localhost:8501
```
