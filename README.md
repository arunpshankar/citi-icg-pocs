# CITI ICG Proof of Concept (PoC) 📁

Repository for CITI ICG's Proof of Concept (PoC). This PoC is designed to address two primary use cases:

* 📊 **Long-form summarization by topic.**
* 🔍 **Detailed examination of derivative contract processing variances**: This delves deeper into the first use case, focusing on highlighting differences between proposed rules and the existing ones.

## 🚀 Getting Started

### 🛠 **Prerequisites**

- **Git** 🌍
- **Python** 🐍 (Version 3.8 or higher recommended)
- **pip** 📦

### 📝 **Setup Instructions**

1. **Clone the Repository** 🔄
   ```bash
   git clone https://github.com/arunpshankar/citi-icg-pocs.git 
   ```

2. **Credentials Setup** 🔐
   
   - Create a folder named `credentials` in the root directory of the cloned repository.
     ```bash
     mkdir credentials
     ```

   - Store your **Google project service account credentials** (as a JSON file) and **OpenAI keys** (as a YAML file) in this folder.
   
   - For OpenAI credentials, create a YAML file named `oai-key.yml` with the following structure:
     ```yaml
     key: YOUR_OPENAI_KEY
     ```

3. **Environment Setup** 🌐

   - **Local Desktop (Native or Virtual Environment)** 💼
     ```bash
     python -m venv venv
     source venv/bin/activate   # On Windows, use: venv\Scripts\activate
     pip install -r requirements.txt
     ```

   - **VertexAI Workbench** 🌟
     
     If you're deploying on the VertexAI Workbench, you can bypass the initial environment variable setup for VertexAI. However, ensure that you still install the necessary packages.
     ```bash
     pip install -r requirements.txt
     ```

---

Thank you for choosing Google Cloud! Feel free to reach out with any questions or feedback. 🌟🚀📈