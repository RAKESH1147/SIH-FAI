# SIH WORKSHOP 
#### NAME : Rakesh K S
#### REGISTER NUMBER : 212224040264

## Intelligent Enterprise Assistant: Enhancing Organizational Efficiency through AI-Driven Chatbot Integration

### Problem ID : SIH1706

### Introduction

* Large public sector organizations receive thousands of employee queries related to HR policies, IT support, leave rules, payroll, company announcements, and internal procedures. Handling these queries manually increases workload on HR and IT teams and slows down employee support.

* An AI-driven enterprise chatbot can automate responses, provide instant information, and reduce manual effort. Using Natural Language Processing (NLP) and Deep Learning, the chatbot can understand employee questions and provide accurate responses.

* This system also supports document processing, security features like Two-Factor Authentication (2FA), and content filtering to maintain professional communication.

### Objectives

The main objectives of the system are:

* Develop an __AI chatbot__ that understands employee queries using NLP.

* Provide responses related to HR policies, IT support, company events, and organizational guidelines.

* Implement document analysis features, including:

    * Document summarization

    * Keyword extraction

* Ensure the chatbot supports at least 5 users simultaneously.

* Maintain response time under 5 seconds.

* Implement Two-Factor Authentication (2FA) for secure login.

* Filter inappropriate language using a bad-word detection dictionary.

### System Architecture

The proposed system consists of multiple components that work together to process user queries and provide responses efficiently.

### User Interface

Employees interact with the chatbot through:

* Web Interface

* Mobile Interface

* Chat Window

Users can:

* Ask questions

* Upload documents

* View summarized results

### Authentication Module (2FA)

Security is implemented using __Two-Factor Authentication__.

__Process__

1. User enters email ID and password.

2. System sends an OTP to the registered email.

3. User enters the OTP.

4. Access to the chatbot is granted.

__Technologies Used__

* Email SMTP server

* OTP generator

### NLP Processing Module

This module processes employee queries and extracts meaning from the text.

__Steps__
__Text Preprocessing__

* Tokenization

* Stop-word removal

* Lemmatization

__Intent Detection__

Identifies the purpose of the question.

```
Query	                            Intent
How many leaves do I have?	        HR Policy
My system is not working	        IT Support
When is the annual meeting?	        Company Events
```
__Entity Extraction__

Extracts important information from the query.

Example:

Query:
Leave policy for maternity leave

Extracted Entity: Maternity Leave

__Technologies__

* Python

* SpaCy

* NLTK

* Transformer models (BERT)

__Knowledge Base__

The chatbot stores information from organizational resources such as:

* HR policy documents

* IT support guides

* Organization announcements

* Employee handbook

Data storage options include:

* JSON files

* Databases

* Vector databases

Example HR policy data:
```json
{
 "leave_policy": "Employees are allowed 20 paid leaves per year"
}
```
### Deep Learning Model

A deep learning model is used for intent classification and response generation.

__Possible Models__

* LSTM

* BERT

* Transformer-based models

__Model Workflow__

User Query
↓
Text Embedding Layer
↓
Deep Learning Model
↓
Intent Prediction
↓
Response Generation

### Document Processing Module

Employees can upload documents for analysis.

__Features__

* Text Extraction

* Document Summarization

* Keyword Extraction

__Text Extraction__

Extract text from:

* PDF files

* Word documents

* Text files

Tools used:

* PyPDF2

* Tesseract OCR

__Document Summarization__

Convert long documents into short summaries.

Example:

Input: 10-page document
Output: 5-10 line summary

Methods used:

* Extractive summarization

* Transformer models (BART / T5)

__Keyword Extraction__

Extract important keywords from uploaded documents.

Example:

Document Topic: Leave Policy

Keywords extracted:

* Leave

* Sick Leave

* Paid Leave

* Policy Rules

Libraries used:

* KeyBERT

* TF-IDF

### Bad Language Filtering

The chatbot filters offensive language using a system-maintained dictionary.

Example dictionary:
```py
bad_words = ["abuse1", "abuse2", "abuse3"]
```
__Process__

User Message
↓
Check against bad-word dictionary
↓

If inappropriate language detected:

__Response:__
"Please use professional language while communicating."

### Scalability and Performance

The chatbot must support a minimum of 5 users simultaneously.

__Methods Used__

* Cloud deployment

* Load balancing

* Efficient model inference

__Technologies__

* FastAPI / Flask

* Docker

* AWS / Azure Cloud

__Performance Goal__

Response time should be less than or equal to 5 seconds per query.

### Technology Stack

```
Component	                        Technology
Frontend	                             React / HTML / CSS
Backend	                             Python Flask / FastAPI
NLP	                                  SpaCy, NLTK
Deep Learning	                         TensorFlow / PyTorch
Database	                              MongoDB / PostgreSQL
Authentication	                    Email OTP
Document Processing	               PyPDF2, OCR
Deployment	                        AWS / Azure / Docker
```
### Working Flow

1. User logs in using Email + OTP (2FA).

2. User sends a query to the chatbot.

3. NLP module processes the query.

4. Deep learning model predicts the intent.

5. Chatbot retrieves the answer from the knowledge base.

6. Response is sent to the user.

7. If a document is uploaded:

* Text is extracted

* Summary is generated

* Keywords are extracted

### Advantages

* Reduces workload on HR and IT teams

* Provides instant employee support

* Improves organizational productivity

* Secure login using 2FA

* Handles document processing automatically

* Scalable for multiple users

### Expected Output

The chatbot will:

* Answer employee queries accurately

* Summarize uploaded documents

* Extract important keywords

* Maintain secure authentication

* Filter offensive language

* Respond within 5 seconds

### Future Enhancements

* Voice-enabled chatbot

* Integration with enterprise software systems

* Multilingual support

* Integration with company internal databases

* AI-powered recommendation system

____The Presentation is as follows:____


https://docs.google.com/presentation/d/18In3_t3eEYVxzxuiQemi_E2EUclyfrYbqb9w9z1awOU/edit?usp=sharing
