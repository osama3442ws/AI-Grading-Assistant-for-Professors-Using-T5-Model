# AI-Powered Grading Assistant

## Overview

This project is an AI-powered grading assistant designed to help professors evaluate student answers based on a given PDF book. The system uses the T5 model from Hugging Face to generate questions from the book, evaluates student answers for these questions, and saves the results in an Excel file.

## Features

- **Text Extraction**: Extracts text from a PDF book.
- **Question Generation**: Generates three questions based on the extracted text.
- **Answer Evaluation**: Evaluates student answers against the book text using TF-IDF and cosine similarity.
- **Result Saving**: Saves student scores and details in an Excel file.

## Requirements

- Python 3.7+
- `transformers` library
- `PyPDF2` library
- `gradio` library
- `scikit-learn` library
- `pandas` library
- `openpyxl` library (for Excel file operations)

You can install the required libraries using pip:

```bash
pip install transformers PyPDF2 gradio scikit-learn pandas openpyxl

## Step 1: Upload the Book and Generate Questions
Upload a PDF book using the file input field.
Click on "Generate Questions" to produce three questions based on the book's content.
The questions will be displayed in the designated text boxes.
## Step 2: Evaluate Student Answers
Enter the student's answers for each of the generated questions.
Provide the student's name and select their academic level from the dropdown menu.
Click "Evaluate Answers and Save Results" to obtain evaluations for each answer and a total score.
The results will be saved in an Excel file named student_scores.xlsx, and a confirmation message will be displayed.
## Code Description
Text Extraction (extract_text_from_pdf): Extracts text from a PDF file.
Question Generation (generate_question_from_text): Uses the T5 model to generate questions based on text segments.
Answer Evaluation (evaluate_student_answer): Assesses student answers against the book text using TF-IDF and cosine similarity.
Result Saving (save_results_to_excel): Saves evaluation results to an Excel file.
Gradio Interface: Provides the user interface for file uploads, question generation, and answer evaluation.
