# -NLP-based-housing-price-prediction-project

# Objective:  Enhancing Property Price Prediction Using Natural Language Processing

**Contributors**: Aisha Mohammad & Suman Attri  
**Date**: May 13, 2025  
**Project Type**: Academic / NLP, Machine Learning, Real Estate Analytics

---

## Project Overview

Traditional property price prediction models often rely only on structured data like square footage, number of rooms, and location. In this project, we explored an underused resource: **property listing descriptions**.

Our goal was to enhance price prediction accuracy by applying **Natural Language Processing (NLP)** techniques to these unstructured textual features and compare the performance to models built on structured data alone.

---

## Technologies & Tools
- **Python** (Pandas, Scikit-learn, Matplotlib, Seaborn)
- **NLP Libraries**: NLTK, spaCy
- **APIs Used**: US Realtor API via RapidAPI
- **Models**: XGBoost, Random Forest
- **NLP Techniques**:
  - Text cleaning
  - TF-IDF Vectorization
  - Named Entity Recognition (NER)
  - Sentiment Analysis (VADER)

---

## Workflow

1. **Data Collection**:  
   - Scraped listing data from the US Realtor API via RapidAPI.

2. **Structured Data Preprocessing**:  
   - Cleaned numerical features (price, sqft, bedrooms, bathrooms, etc.)

3. **NLP Preprocessing**:  
   - Removed stopwords, lowercased text, lemmatization
   - Applied **TF-IDF** to vectorize descriptions

4. **NER & Sentiment Analysis**:  
   - Extracted entities such as brand names, neighborhoods, and amenities
   - Used VADER to evaluate emotional tone in descriptions

5. **Modeling**:
   - Compared models trained on structured data vs combined structured + NLP features
   - Evaluated using RMSE and R²

---

## Results

- **Prediction Accuracy** improved by **16%** when including NLP features from descriptions
- **XGBoost** outperformed Random Forest by **6%**, likely due to better handling of sparse TF-IDF matrices and sequential learning
- **Sentiment features** were removed due to bias, but NER and TF-IDF were retained

---

## Key Insights

- Listing descriptions contain valuable **pricing signals** such as luxury terms, neighborhood names, and feature mentions (e.g., "chef’s kitchen", "hardwood floors")
- **Textual data** helps uncover hidden value not reflected in numeric fields

---

## Business Impact

- **More accurate pricing models** improve real estate valuation, investor decision-making, and property ranking for agents or platforms
- Demonstrates potential of combining structured + unstructured data in predictive modeling

---

## Future Work

- Integrate image analysis of property photos
- Improve sentiment analysis using deep learning (e.g., BERT)
- Fine-tune NER using domain-specific vocabularies

---


## Contact

**Aisha Mohammad**  
📧 aisha.datatech@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/aisha-mohammad-26600b2a2/)  
