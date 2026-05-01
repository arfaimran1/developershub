# Zero-Shot Support Ticket Classification using LLM

## Overview

This project uses a **Zero-Shot Large Language Model (LLM)** to automatically classify customer support tickets into relevant categories without task-specific training.

The model leverages **facebook/bart-large-mnli** from Hugging Face for zero-shot text classification.

---

## Objective

Automatically assign support tags to incoming customer tickets such as:

* Network Issue
* Account Issue
* Billing Issue
* App Bug
* General Support

---

## Technologies Used

* Python
* Hugging Face Transformers
* PyTorch
* Pandas

---

## Model Used

* **facebook/bart-large-mnli**

### Why This Model?

This model is trained for **Natural Language Inference (NLI)** and can perform **zero-shot classification**, allowing it to classify text into unseen categories without additional training.

---

## Dataset

Sample customer support tickets are manually provided for demonstration.

Example Tickets:

* My internet is not working since morning
* I want to reset my password
* Payment failed during checkout process
* App is crashing frequently when I open it
* How can I update my profile information

---

## How It Works

1. Load zero-shot classification pipeline
2. Define candidate support labels
3. Pass each support ticket to model
4. Retrieve:

   * Top predicted tag
   * Top 3 probable tags
   * Confidence scores

---

## Output Format

Results are displayed in a Pandas DataFrame containing:

* Original Ticket
* Predicted Top Tag
* Top 3 Suggested Tags
* Confidence Scores

---

## How to Run

### Install Dependencies

```bash id="z1y4co"
pip install transformers torch pandas
```

### Run Script

```bash id="m0ykod"
python zero_shot_ticket_classifier.py
```

---

## Sample Output

| Ticket                                   | Top Tag       |
| ---------------------------------------- | ------------- |
| My internet is not working since morning | Network Issue |
| I want to reset my password              | Account Issue |
| Payment failed during checkout process   | Billing Issue |

---

## Project Workflow

1. Define Support Tickets
2. Define Candidate Labels
3. Load Zero-Shot LLM
4. Predict Ticket Categories
5. Display Results in Table

---

## Future Improvements

* Add Gradio/Streamlit Web Interface
* Use real customer ticket dataset
* Fine-tune model for domain-specific support tickets
* Integrate with CRM/Helpdesk systems

---

## Author

Arfa Imran
