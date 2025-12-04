# Ethics & Transparency Framework

## Project Overview
This project focuses on detecting AI-generated vs human-written news articles using ML and NLP.  

**Datasets used:**
- AI-Generated Tech News Summaries (Kaggle)
- Fake and True News Dataset (Figshare/Kaggle)
- Human vs LLM Text Corpus (Kaggle)
- MediaBias Dataset (Kaggle)
- Additional GitHub datasets (Sycophantic_LLaMA, Qbias)

## Machine Learning Implementation
**Preprocessing:**
- Remove missing values
- Text cleaning (lowercasing, punctuation removal)
- Tokenization: TF-IDF / SentencePiece
- Train-test split (80/20)

**Models Implemented:**
- Logistic Regression
- Random Forest
- Naive Bayes

### ML Results Summary

#### Fake vs True News
| Model | Accuracy | Precision | Recall | F1-score |
|-------|---------|-----------|--------|----------|
| Logistic Regression | 0.9922 | 0.99 | 0.99 | 0.99 |
| Random Forest | 0.9990 | 1.00 | 1.00 | 1.00 |
| Naive Bayes | 0.9382 | 0.94 | 0.94 | 0.94 |

#### AI vs Human Tech News
| Model | Accuracy | Precision | Recall | F1-score |
|-------|---------|-----------|--------|----------|
| Logistic Regression | 0.9849 | 0.98 | 0.99 | 0.98 |
| Random Forest | 0.9974 | 1.00 | 1.00 | 1.00 |
| Naive Bayes | 0.9263 | 0.93 | 0.93 | 0.93 |

## Ethical Considerations
- Dataset bias
- Model bias
- Feature bias

## Guidelines for Responsible Interpretation
- Only act on high-confidence predictions
- Use predictions as **assistance**, not definitive
- Review feature importance
- Cross-check sources

## Transparency Metrics
- Confidence thresholds
- Uncertainty quantification
- Subgroup performance
- Feature interpretability

## Recommendations for Media Literacy
- Highlight that AI detection is probabilistic
- Encourage verification from multiple sources
- Share common model errors
- Provide examples of linguistic features

## Deliverables
- Trained models (`models/`)
- Datasets (`data/`)
- Notebooks (`notebooks/`)
- Scripts (`src/`)
- Ethics framework (`ethics_transparency.md`)
- Streamlit app

