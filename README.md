# 🇸🇰 Slovak Parliamentary Speech Analysis

A project focused on analyzing speeches from parliamentary sessions to extract insights,
topics, political views and other fun stuff.


## Project Overview

This project performs text analysis using various commercially available LLMs.

*   Score and analyze political views.
*   ...
*   ...


## Political views analysis


This analysis uses LLMs to assess and score politicians' stances within their parliamentary speeches.
Speeches are scored across predefined dimensions critical to contemporary Slovak politics:
*   **The sociocultural dimension** maps views from liberal (individual rights, progressive change) 
    to conservative (traditional values, national norms).
*   **The geopolitical dimension** maps alignment from pro-Western (EU/NATO integration, Western ties) 
    to pro-Eastern / sovereignist (national sovereignty, skepticism of Western alliances).
*   **The corruption and rule of law dimension** maps stances from actively promoting anti-corruption 
and transparency to tolerating clientelism and the status quo.

### Methodology

The core methodology involves analyzing each parliamentary speech using multiple LLMs. 
Specifically, every speech was independently evaluated by four distinct models: Gemini 2.5 Flash, Claude 3.5 Haiku, 
GPT-4.1 mini, and DeepSeek V3. 
The scores from these models were then aggregated to provide a more reliable measure of the expressed political stances.
Full prompt and preprocessing used can be found in [it can't](#todo).

### Results

Detailed results can be found and painfully read from [Political_speech_analysis_political_views.ipynb](Political_speech_analysis_political_views.ipynb).
Easily accessible 3D scatter plot visualization of current politician's political stances can be found [here](https://thecodecook.github.io/sk_parliamentary_speech_analysis/politicians_views_dist/).

## Data Source

The primary data for this project consists of parliamentary speeches transcripts obtained from:
*   **Source:** Scraped NRSR speeches
*   **Link:** https://www.nrsr.sk
*   **Period Covered:** Current election cycle 2023 - (2027?)
*   **Using:** [michalfapso/nrsr.sk.parser](https://github.com/michalfapso/nrsr.sk.parser)

