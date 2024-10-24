# Constructing-Structured-Database-from-Unstructured-Legal-Documents
This project aims to compare 3 methods for the transformation of unstructured textual content in Hebrew legal documents into structured data

## Install & Dependencies

To set up the environment and install the necessary dependencies for this project, follow the steps below:

### 1. Clone the Repository
First, clone the repository from GitHub:

```bash
git clone https://github.com/shay681/Constructing-Structured-Database-from-Unstructured-Legal-Documents.git

cd Constructing-Structured-Database-from-Unstructured-Legal-Documents
```

### 2. Create a Virtual Environment (Optional but recommended)
It's a good practice to create a virtual environment to manage dependencies. Use the following command to create and activate a virtual environment:

```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
# For Windows:
venv\Scripts\activate
# For macOS/Linux:
source venv/bin/activate
```

### 3. Install Dependencies
Install the required dependencies using the `requirements.txt` file provided:

```bash
pip install -r requirements.txt
```

### 4. Install CUDA (For GPU Acceleration)
If you're running the models on a GPU, ensure that CUDA is installed. You can check CUDA installation instructions from [NVIDIA's official website](https://developer.nvidia.com/cuda-downloads).

Make sure the CUDA version matches your GPU and driver requirements.


## Datasets
All datasets that are used in this project can be found here:
[Datasets](https://huggingface.co/datasets?sort=trending&search=shay681)
| Dataset | Description |
|   ---   |     ---     |
| Legal_Clauses | Dataset containing legal clauses extracted from Hebrew legal documents |
| Precedents | Dataset of legal precedents from Hebrew court decisions |
| Inference_Legal_Clauses | Inference dataset for predicting legal clauses in unstructured text |
| Inference_Precedents | Inference dataset for predicting legal precedents in unstructured text |


## Models
All models that are trained and used in this project can be found here:
[Models](https://huggingface.co/models?search=shay681)

| Model Name | Desciption |
|    ---     |    ---     |
| shay681/HeBERT_finetuned_Legal_Clauses |	HeBERT model fine-tuned on legal clauses |
| shay681/HeBERT_finetuned_Precedents |	HeBERT model fine-tuned on precedents |
| shay681/Text2Text_Legal_Clauses_finetuned_model |	Text-to-text model fine-tuned on legal clauses |
| shay681/Text2Text_Precedents_finetuned_model |	Text-to-text model fine-tuned on precedents |


### Tested Platform
- hardware
  ```
  CPU: Intel(R) Xeon(R) CPU E5-2687W v4 @ 3.00GHz
  GPU: NVIDIA TESLA P40-2Q (24GB)
  ```