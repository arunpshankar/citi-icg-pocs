# POC for CITI ICG

---

This Proof of Concept (POC) is aimed at finding the differences in the processing of derivative contracts between proposed rules and existing rules (use case 2).

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
---