# Passive-Aggressive Email Rewriter

This repository has an NLP pipeline that detects email tones with BERT and rewrites them passive-aggressively using GPT-2 fine-tuned with LoRA (Low-Rank Adaptation).

## Project Overview
The tool performs two tasks:
1. **Tone Detection**: Fine-tuned `bert-base-uncased` classifies emails as positive, neutral, or negative.
2. **Rewriting**: Fine-tuned `gpt2` with LoRA generates passive-aggressive versions.

## Dataset
- **File**: `tone_dataset.csv`
- **Columns**: 
  - `original_email`: Input email.
  - `Tone`: Label (positive, neutral, negative).
  - `passive-aggressiv`: Target rewrite.
- **Size**: 147 samples.

## Installation
1. Clone the repo:
   ```bash
   git clone https://github.com/vivekschaurasia/Passive-Aggressive-Email-Rewriter.git
   cd passive-aggressive-email-rewriter
