# CodePath: A Personalized Learning Pathways and Course Recommendations Chatbot

## Group Members:

*   Geron Simon A. Javier
*   Mhar Andrei C. Macapallag
*   Seanrei Ethan M. Valdeabella

## Section:

*   BSCS 3B - IS

## Submitted to:

*   Mr. Mark Bernardino
*   Mrs. Mia Villarica

## Table of Contents

1. [Introduction](#introduction)
2. [Project Overview](#project-overview)
4. [Code](https://github.com/simon-javier/CSST102-Final-Project/tree/main/code)
5. [Datasets](https://github.com/simon-javier/CSST102-Final-Project/tree/main/data)
6. [Weekly Progress Report](https://github.com/simon-javier/CSST102-Final-Project/tree/main/weekly-progress-report)
7. [Documentation](https://github.com/simon-javier/CSST102-Final-Project/tree/main/documentation)
8. [Usage](#usage)
9. [Model Evaluation](#model-evaluation)
10. [Challenges](#challenges)
11. [Future Improvements](#future-improvements)
12. [Conclusion](#conclusion)
13. [Contributors](#contributors)


## Introduction

This repository contains the code and resources for **CodePath**, a chatbot designed to provide personalized learning pathways and course recommendations for computer science students. The project was developed by Geron Simon A. Javier, Mhar Andrei C. Macapallag, and Seanrei Ethan M. Valdeabella of BSCS 3B - IS as a part of their coursework.

## Project Overview

CodePath is an advanced chatbot that leverages a Transformer-based neural network and causal language modeling to assist computer science students. It is designed to:

*   Understand user queries related to computer science topics.
*   Provide tailored advice based on the student's knowledge level.
*   Generate coherent and contextually relevant responses.
*   Handle special commands like `reset`, `analyze`, `help`, and `feedback`.
*   Maintain conversation history for context.
*   Detect user intent (e.g., greeting, question, command).

## Usage

1. **Prerequisites:**
    *   Python 3.8+
    *   A Hugging Face account and API token (for accessing the model and dataset)

2. **Installation:**
    *   Clone this repository:
        ```bash
        git clone https://github.com/simon-javier/CSST102-Final-Project.git
        cd CSST102-Final-Project/code/Codepath-GUI-Flask
        ```
    *   Install the required packages:
        ```bash
        pip install -r requirements.txt
        ```

3. **Set up environment variables:**
    *   Create a `.env` file in the root directory.
    *   Add your Hugging Face token:
        ```
        HUGGINGFACE_TOKEN=<your_huggingface_token>
        ```

4. **Run the application:**
    ```bash
    python app.py
    ```
    or
   ```bash
   python -m flask run
   ```
    This will start the Flask development server. Access the chatbot in your web browser at `http://127.0.0.1:5000/`.

6. **Web Interface**
    *  On the homepage, enter the Hugging Face repository name and the commit hash of the model you want to use.
    *  Click "Load Model" to load the selected model.
    *  Start chatting with the chatbot in the chat interface.

7. **Special Commands**
    *   `reset` or `clear`: Clears the conversation history.
    *   `analyze` or `stats`: Provides an analysis of the conversation.
    *   `help` or `commands`: Displays available commands.
    *   `feedback`: Allows you to provide feedback on the chatbot's performance.
    *   `quit`, `exit`, or `bye`: Ends the chat session and saves the conversation history.

## Model Evaluation

The model's performance was evaluated using various metrics:

*   **Accuracy:** 0.9998
*   **Precision:** 0.8333
*   **Recall:** 1.0000
*   **F1 Score:** 0.9091
*   **Average BLEU Score:** 0.0990
*   **AUC-ROC:** 1.00

These results demonstrate the model's strong ability to classify relationships between inputs and outputs, generate relevant responses, and understand the context of conversations. The `Evaluation.ipynb` notebook provides more detailed analysis and visualizations.

## Challenges

*   **Data Quality and Diversity:** Creating a synthetic dataset that accurately reflects real-world queries and covers a wide range of topics and difficulty levels.
*   **Hyperparameter Tuning:** Finding the optimal balance between model generalization and specialization.
*   **Context Management:** Maintaining coherence in extended conversations.
*   **Intent Recognition:** Accurately detecting user intent, especially in ambiguous or multi-faceted queries.
*   **Response Quality:** Generating high-quality, non-repetitive responses that adapt to the user's knowledge level.
*   **Ethical Considerations:** Implementing safeguards against generating inappropriate content.
*   **Scalability and Performance:** Ensuring smooth user experience with concurrent users.
*   **Continuous Learning:** Keeping the chatbot updated with the latest computer science knowledge.
*   **GPU Limitations:** The initial dataset size and model complexity led to resource constraints on Google Colab.

## Future Improvements

*   Enhance data quality and diversity.
*   Refine the model's fine-tuning process.
*   Expand the chatbot's capabilities (e.g., add more advanced features, support more complex queries).
*   Improve context management for longer conversations.
*   Explore techniques for better intent recognition.
*   Implement a more robust feedback mechanism.

## Conclusion

CodePath is a significant step towards creating an advanced AI-powered learning assistant for computer science. It demonstrates the potential of Transformer-based models and causal language modeling in educational applications. The project provides a solid foundation for future development and expansion.

## Contributors

*   Geron Simon A. Javier
*   Mhar Andrei C. Macapallag
*   Seanrei Ethan M. Valdeabella


