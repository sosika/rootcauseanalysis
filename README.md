# Root Cause Analysis Tool

This project provides a framework for performing root cause analysis using OpenAI's API. It integrates Python libraries to streamline data analysis and automate the process of identifying the underlying causes of issues in datasets.

## Features
- Automated root cause analysis using AI models.
- Integration with OpenAI API for advanced data interpretation.
- Simple and modular code for easy customization.

## Prerequisites
- Python 3.7+
- OpenAI API Key
- Required libraries: `openai`, `json`, `IPython`, `re`

## Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/rootcauseanalysis.git
   cd rootcauseanalysis
   ```
2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Setup
1. Store your OpenAI API key securely.
2. Update the `helper.py` file to retrieve your API key:
   ```python
   from helper import get_openai_api_key
   openai_api_key = get_openai_api_key()
   ```

## Usage
Here are examples of how to use the tool:

### Example 1: Importing Libraries and Setting Up API Key
```python
# Warning control
import warnings
import openai
warnings.filterwarnings('ignore')

# Import OpenAI key
from helper import get_openai_api_key
openai_api_key = get_openai_api_key()
```

### Example 2: Initializing OpenAI Client
```python
import json
from IPython.display import display, Markdown, HTML
from openai import OpenAI
import re

client = OpenAI(api_key=openai_api_key)
O1_MODEL = 'o1-mini'
```



