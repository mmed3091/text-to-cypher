# Text-to-Cypher Pipeline

This project automates the generation, correction, and evaluation of Cypher queries for knowledge graph construction from Wikipedia-style text. It uses multiple LLMs (OpenAI, Gemini, Claude, Cohere) to generate and benchmark queries based on accuracy and correctness.

## Process

- Scrape and preprocess text from URLs
- Generate Cypher queries using:
  - OpenAI (GPT-4)
  - Google Gemini (Pro)
  - Cohere (Command R+)
  - Anthropic Claude (Haiku)
- Detect syntax and semantic issues in queries
- Auto-correct errors using LLMs
- Evaluate performance across models with metrics
- Output detailed summaries and benchmarks

## Dependencies

```
pip install -r requirements.txt
```
## Setup

1. Clone repository
2. Create a .env file in the root directory and add your API keys like so:

```
OPENAI_API_KEY=openai_key
GOOGLE_API_KEY=google_key
COHERE_API_KEY=cohere_key
ANTHROPIC_API_KEY=anthropic_key
```
3. Add URLs of choice to the links.txt file, one URL per line

## Usage

Navigate to folder the main script (pipeline.py)  is in and run it:
```
python pipeline.py
```

## Output

JSON and text files containing results and metrics ready for evaluation.


