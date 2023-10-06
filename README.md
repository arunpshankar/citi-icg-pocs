# CITI ICG

This repository contains all the essential notebooks and supplementary files assembled for CITI ICG's Proof of Concept (PoC). The PoC targets two specific use cases:

* 1/ Long-form summarization by topic.
* 2/ An expanded version on use case 1/ focusing on identifying the variances in the processing of derivative contracts when comparing proposed rules to the current ones.

## Setup

### Prerequisites

- Git
- Python (recommended version 3.8 or higher)
- pip

### Steps

1. **Clone the Repo**
   ```bash
   git clone https://github.com/arunpshankar/citi-icg-pocs.git 
   ```

2. **Credentials Folder**
   Create a folder named `credentials` in the root directory of the cloned repository.
   ```bash
   mkdir credentials
   ```

   Save your service account credentials for your Google project and OpenAI keys (as a yml file) in this folder.

3. **Environment Setup**
   - **Local Desktop - Native or Virtual Environment (preferred)**
     ```bash
     python -m venv venv
     source venv/bin/activate   # On Windows, use: venv\Scripts\activate
     pip install -r requirements.txt
     ```

   - **VertexAI Workbench**
     If you're running on VertexAI Workbench, you can ignore the initial setup of setting up environment variables for VertexAI. However, still ensure you install the required packages:
     ```bash
     pip install -r requirements.txt
     ```