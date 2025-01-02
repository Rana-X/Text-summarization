# Text-summarization using Pegasus (HuggingFace)
Description
A text summarization model based on Pegasus, fine-tuned on the SAMSum dataset to automatically generate concise summaries from messenger-style conversations. This model helps convert long chat conversations into brief, coherent summaries.
Key Features

Processes chat/messenger style conversations
Generates human-readable summaries
Fine-tuned on conversational data
Uses ROUGE metrics for evaluation

Quick Start
pythonCopyfrom transformers import pipeline

summarizer = pipeline("summarization", model="[your-huggingface-repo]")
text = """
[Your conversation here]
"""
summary = summarizer(text, max_length=130, min_length=30)
Model Details

Base Model: Pegasus
Dataset: SAMSum
Task: Conversation Summarization
Language: English

Limitations

Best suited for conversational text
Optimal performance on messenger-style dialogues
Summary length limited to model parameters
