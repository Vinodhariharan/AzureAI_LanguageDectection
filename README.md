# Azure AI Fundamentals - Text Analytics Exercise

This project demonstrates how to use **Azure AI's Text Analytics API** to perform natural language processing tasks such as **language detection**, **sentiment analysis**, **key phrase extraction**, and **entity recognition** on text documents.

This is part of a hands-on exercise to prepare for the **Microsoft AI-900: Azure AI Fundamentals** certification.

## Project Structure

```
.
├── reviews/              # Folder containing text files to be analyzed
├── .env                  # Environment file with Azure AI credentials
├── analyze_reviews.py    # Main script for analyzing text documents
├── README.md             # Project documentation
```

## Features

This script uses Azure's `TextAnalyticsClient` to perform the following tasks on each text file in the `reviews/` folder:

* **Detect Language**
* **Analyze Sentiment**
* **Extract Key Phrases**
* **Recognize Named Entities**
* **Recognize Linked Entities**

## Prerequisites

* Python 3.7+
* Azure subscription with **Azure Cognitive Services** enabled
* Provisioned **Text Analytics** resource in Azure

## Installation

1. Clone the repository or copy the script.
2. Install dependencies:

```bash
pip install azure-ai-textanalytics python-dotenv
```

3. Create a `.env` file in the project root:

```env
azureAI_Endpoint=https://<your-resource-name>.cognitiveservices.azure.com/
azureKey=<your-text-analytics-key>
```

4. Add `.txt` files to the `reviews/` folder for analysis.

## Usage

Run the script:

```bash
python analyze_reviews.py
```

Each file's results will be printed to the console, including detected language, sentiment, key phrases, named entities, and linked entities.

## Learn More

* [AI-900 Certification Guide](https://learn.microsoft.com/en-us/certifications/exams/ai-900/)
