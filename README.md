# MedChat Repository

Welcome to the MedChat repository! This project focuses on optimizing contextual augmentation for generative AI performance in medical chatbot responses. Specifically, it explores the use of large language models (LLMs) to answer questions related to theranostics and nuclear medicine.
The LLMs used in this experiment are:

- GPT-4
- GPT-4o
- Gemini 1.5
- Claude 3 Opus
- Command R+


## Repository Structure

The repository is organized into the following main directories:

- **Evaluation**
- **NoContext**
- **WithContext**

### NoContext

In the `NoContext` directory, you will find the answers provided by the LLMs without any additional context. These responses are generated purely based on the pre-trained knowledge of the models. 

### WithContext

The `WithContext` directory is further divided into two subdirectories: `NaiveRAG` and `AdvancedRAG`.

- **NaiveRAG**: This subdirectory contains the answers generated by the LLMs using additional context files from the `context_files` folder. These context files provide supplementary information to help the models generate more accurate responses.

- **AdvancedRAG**: In addition to the context files, the AdvancedRAG approach incorporates advanced techniques such as HyDE and LLM reranking to refine the answers further.

### Evaluation

The `Evaluation` directory contains scripts and results for evaluating the performance of the LLM-generated answers. We used the Tonic Validate framework to evaluate the answers according to several metrics, ensuring a comprehensive assessment of the model performance.

## Usage

To use this repository, follow these steps:

1. **Clone the repository**:
    ```sh
    git clone https://github.com/piakoller/MedChat.git
    cd MedChat
    ```

2. **Explore the datasets**: 
    - The `Evaluation-Questions.csv` file contains the questions related to theranostics and nuclear medicine.
    - The `context_files` folder contains additional context documents used for the `WithContext` approaches.

3. **Review the answers**:
    - Answers generated without context can be found in the `NoContext/csv-NoContext` folder.
    - Context-augmented answers are available in the `WithContext/NaiveRAG/csv-NaiveRAG` and `WithContext/AdvancedRAG/csv-AdvancedRAG` folders.

4. **Evaluate the models**:
    - Navigate to the `Evaluation` folder to see the evaluation scripts and results using the Tonic Validate framework.

---

We hope you find this repository useful for your research and development in the field of medical chatbots and generative AI. If you have any questions or need further assistance, please don't hesitate to contact us.

Happy coding!
