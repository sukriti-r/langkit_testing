# LangKit Testing Environment Setup

This README provides instructions for setting up a Python 3.9 environment with LangKit and the required dependencies.

## Prerequisites

- Python 3.9
- pip (Python package installer)

## Setup Instructions

```bash
pip install virtualenv
virtualenv --python=python3.9 langkit_env

# On Windows:
langkit_env\Scripts\activate
# On macOS/Linux:
source langkit_env/bin/activate

pip install langkit[all]
pip install numpy==1.24.0
```

## API Key Configuration

```python
import os
os.environ["OPENAI_API_KEY"] = "<YOUR OPENAI API KEY>"
```

## Running the Script

```bash
python langkit_demo_test.py
```
