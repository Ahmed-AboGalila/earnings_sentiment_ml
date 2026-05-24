# Earnings Call Sentiment Analysis 📈

## Project Overview
Analyzing Earnings Call transcripts using NLP and FinBERT 
sentiment analysis to predict stock market reactions after 
quarterly earnings releases.

## Dataset
- 8 real Earnings Call quotes from Apple, Microsoft, 
  Goldman Sachs and Tesla
- Stock price reactions sourced via Yahoo Finance API

## Workflow
- Loaded and structured real Earnings Call quotes
- Applied FinBERT (Finance-specific NLP model) for sentiment classification
- Compared sentiment predictions with actual stock price reactions
- Visualized results with Matplotlib

## Results
- FinBERT correctly classified 8/8 earnings call sentiments
- Key finding: All positive sentiments corresponded with rising 
  stock prices, all negative sentiments with falling prices
- Important limitation: FinBERT confidence score does not 
  correlate with the magnitude of stock price movement — 
  Tesla and Microsoft showed strong reactions despite 
  moderate confidence scores

## Key Learnings
- NLP models like FinBERT can reliably detect sentiment direction 
  in financial texts
- However, market reaction magnitude depends on many more factors 
  beyond sentiment — analyst expectations, macro environment, 
  and prior guidance all play a role
- This highlights the importance of combining NLP with 
  quantitative models for real trading decisions

## Tech Stack
- Python, Pandas, HuggingFace Transformers, FinBERT, 
  Matplotlib, Yahoo Finance API

## Why This Matters for Finance
Hedge funds and asset managers increasingly use NLP models 
to analyze earnings calls, analyst reports and central bank 
statements in real time. FinBERT enables finance professionals 
to systematically extract sentiment signals that would take 
humans hours to process manually.
