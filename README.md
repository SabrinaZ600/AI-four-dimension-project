# AI Visibility vs. Brand Strength
## Why Do Strong Brands Fail to Be Recommended by AI?
### A Multi-Source Framework Integrating Social Media Analytics and Large Language Models
---
## Project Overview
Large Language Models (LLMs) are rapidly becoming an important source of product recommendations. However, brands with strong market performance are not always recommended by AI systems.

This project investigates the gap between **real-world brand strength** and **AI recommendation visibility** by proposing a four-dimensional evaluation framework that integrates:

- Brand Strength
- Product Strength
- Marketing Strength
- AI Visibility

The framework combines large-scale social media analytics, Natural Language Processing (NLP), and Large Language Model (LLM) evaluation to quantify the relationship between market performance and AI recommendation behavior.

---

## Research Question

> Why are some strong brands frequently ignored by AI recommendation systems while weaker brands receive greater AI exposure?
---
## Research Framework

                    Research Question

     Why Do Strong Brands Fail to Be Recommended by AI?

                             │
                             ▼

           Multi-Source Brand Evaluation Framework
           

 ┌────────────────────────────────────────────────────────────┐
 │                                                            │
 │                Real-World Brand Strength                   │
 │                                                            │
 │  ┌────────────┐     ┌────────────┐     ┌──────────────┐    │
 │  │   Brand    │     │  Product   │     │   Marketing  │    │
 │  │  Strength  │     │  Strength  │     │   Strength   │    │
 │  └────────────┘     └────────────┘     └──────────────┘    │
 │                                                            │
 └────────────────────────────────────────────────────────────┘
 
                             │
                             │
                             ▼

               Large Language Model Evaluation

                             │

             14 Standardized Recommendation Prompts

                             │

                             ▼

                  AI Visibility Measurement

                        Mention Rate
                        Average Rank
                        Top-1 Rate
                        Top-3 Rate

                             │

                             ▼

                 AI Blind Spot Identification

                     AI Over-recommended
                     AI Under-recommended
                     AI Aligned

The proposed framework evaluates brands from four complementary perspectives before comparing them with AI recommendation performance.

---

# Methodology

## Stage 1 — Brand Strength

Social media discussions were collected from a commercial media monitoring platform covering major Chinese social media platforms.

Three indicators were constructed:

| Dimension | Indicator |
|------------|-----------|
| Brand Awareness | Total Posts |
| Brand Reputation | Positive Sentiment Ratio |
| Brand Trust | Trust Score (LLM-based evaluation) |

Brand trust was extracted using the **Qwen2.5-0.5B-Instruct** model through structured prompt engineering.

---

## Stage 2 — Product Strength

Consumer discussions were analyzed at the sentence level.
Seven product dimensions were evaluated:
- Sound Quality
- Active Noise Cancellation
- Comfort
- Connectivity
- Battery
- Design
- Price
Sentence-level sentiment analysis was performed using

> DistilBERT Multilingual Sentiment Model

Each dimension received a score from 1–5.

The average score represents the overall Product Strength.

---

## Stage 3 — Marketing Strength

Marketing performance was measured using the proposed

> Digital Evidence Strength Index (DESI)

DESI integrates four dimensions:

| Indicator | Weight |
|-----------|---------|
| Information Volume | 35% |
| Platform Diversity | 25% |
| Platform Entropy | 20% |
| Temporal Stability | 20% |

---

## Stage 4 — AI Visibility

Fourteen standardized recommendation prompts were submitted to an LLM.

Metrics extracted include:

- Mention Rate
- Average Ranking
- Top-1 Appearance
- Top-3 Appearance

These indicators were normalized into a unified AI Visibility Score.

---

# Statistical Analysis

The following analyses were conducted:

- Correlation Analysis
- Logistic Regression
- AI Blind Spot Detection
- Prompt-Level Recommendation Analysis

---

# Repository Structure

```
AI-Brand-Visibility/

├── README.md
├── LICENSE
├── requirements.txt

├── notebooks/
│
│   ├── 01_Brand_Strength.ipynb
│   ├── 02_Product_Strength.ipynb
│   ├── 03_Marketing_Strength.ipynb
│   ├── 04A_LLM_Response_Collection.ipynb
│   ├── 04B_Response_Processing.ipynb
│   ├── 04C_AI_Visibility.ipynb
│   └── 05_Statistical_Analysis.ipynb

├── data/
│
│   ├── sample_data.csv
│   └── README.md

├── outputs/
│
│   ├── AI_Visibility_Score.csv
│   ├── correlation_matrix.csv
│   ├── analysis_dataset.csv
│   ├── brand_rankings.csv
│   └── Brand_Strength.csv

├── figures/
│
│   ├── research_framework.png
│   ├── methodology_pipeline.png
│   ├── correlation_heatmap.png
│   ├── regression_coefficients.png
│   ├── AI_blindspot.png
│   └── recommendation_heatmap.png

└── docs/
```
---

# Technologies

Python

Pandas

NumPy

Scikit-learn

Statsmodels

Transformers

Hugging Face

Qwen2.5

DistilBERT

Matplotlib

Google Colab

OpenAI Compatible API

---

# Key Results

Major findings include:

- Brand trust exhibits the strongest positive relationship with AI recommendation frequency.
- Marketing strength improves online visibility but contributes less to AI recommendation performance.
- Several brands exhibit significant discrepancies between market strength and AI visibility.
- AI recommendation systems demonstrate measurable recommendation bias toward certain brands.

---

# Example Outputs

### Correlation Analysis

<p align="center">
<img src="figures/correlation_heatmap.png" width="650">
</p>

---

### AI Blind Spot

<p align="center">
<img src="figures/AI_blindspot.png" width="650">
</p>

---

### Logistic Regression

<p align="center">
<img src="figures/regression_coefficients.png" width="650">
</p>

---

### Prompt-Level Recommendation Heatmap

<p align="center">
<img src="figures/recommendation_heatmap.png" width="700">
</p>

---

# Data Availability

The original social media dataset is proprietary and cannot be publicly released.

A sample dataset is provided for demonstration purposes.

---
