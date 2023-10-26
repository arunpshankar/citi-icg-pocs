# CITI ICG Proof of Concept 📁

Welcome to the repository for CITI ICG's Proof of Concept (PoC). This PoC is designed to comprehensively address two primary use cases:

* 📊 **Long-form summarization by topic**: Extracting the essence of extensive documents and presenting them in a concise manner.
* 🔍 **Detailed examination of derivative contract processing variances**: A deeper dive into the first use case, this focuses on highlighting the differences between proposed rules and existing ones, ensuring clarity and accuracy.

## 🚀 Getting Started

### 🛠 **Prerequisites**

- **Git** 🌍: Ensure you have Git installed to clone the repository.
- **Python** 🐍: Version 3.8 or higher is recommended for compatibility.
- **pip** 📦: Required for installing the necessary packages.

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

   - Store your **Google project service account credentials** (JSON format) and **OpenAI keys** (YAML format) in this folder.
   
   - For OpenAI credentials, use the following YAML structure in a file named `oai-key.yml`:
     ```yaml
     key: YOUR_OPENAI_KEY
     ```

3. **Environment Setup** 

   - **Local Desktop (Native or Virtual Environment)** 💼
     ```bash
     python -m venv venv
     source venv/bin/activate   # On Windows, use: venv\Scripts\activate
     pip install -r requirements.txt
     ```

   - **VertexAI Workbench** 
     
     If deploying on the VertexAI Workbench, bypass the initial environment variable setup for VertexAI. Ensure the necessary packages are installed:
     ```bash
     pip install -r requirements.txt
     ```

## 📂 Repository Structure

- **Approach-1**: This folder houses notebooks demonstrating the use of RAG (Retrieval Augmented Generation) with VertexAI's `text-bison 8k model (palm2)`. The aim is to identify differences, aligning with use case 2. It also contains notebooks comparing the results against the OpenAI GPT-4 model. Additionally, there's code to preprocess PDF documents using VertexAI DocumentAI and Vision AI.

- **Approach-2**: Here, you'll find notebooks that adopt a recursive summarization strategy, bypassing RAG, and utilizing long-context models in a multi-level map-reduce pattern. We juxtapose the `PaLM text-bison 32k` model against `ChatGPT 16k` and `GPT-4 8k` models, focusing primarily on long-form summarization. In the culmination, a pipeline is crafted using the 8k and 32k `text-bison` models, leveraging the document's table of contents to refine and enhance the summary, targeting use cases 1 and 2.

- **Claude2 Summarizer**: This folder incorporates the `Claude2 100k` model to approach the problem, offering another perspective.

- **DocumentAI Summarizer**: An innovative feature of DocumentAI, this can be directly employed to construct summarizers for extensive documents.

By juxtaposing the results from various experiments, it becomes evident that the most optimal outcomes are achieved when employing a multi-level map-reduce pipeline using VertexAI's `text-bison 8k and 32k models`.

---

Thank you for choosing Google Cloud! We're here to assist. Please don't hesitate to reach out with any inquiries or feedback.