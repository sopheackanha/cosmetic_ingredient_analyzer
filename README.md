# Cosmetic Ingredient Safety Analyzer
The Cosmetic Ingredient Safety Analyzer is a lightweight machine learning system designed to help consumers assess the safety of cosmetic ingredients. By analyzing ingredients in terms of text and images provided by user, it flags potentially harmful components based on data from authoritative public health database (EU CosIng Annex II). This system bridges the gap between complex chemical information and accessible consumer knowledge, aiming to protect user health, increase awareness, and increase ingredient transparency in the beauty industry.
## Problem Statement
Most people are not aware of the scientific terms or chemical ingredients in beauty products. Doing research one by one about those ingredients is inconvenient and time consuming. In some cases, the manufacturer might use alternative terms for the ingredient, which can be confusing for non-expert consumers.Thus, people might just pick whatever products that are on trend without knowing its side effects or whether they are suitable for them, leading to further problems such as allergy, cancer, and so on.
## Installation
```
python -m venv venv
```
```
venv\Scripts\activate
```
```
pip install -r requirements.txt
```
## Contribution
My specific work on this project included:
- Data collection: downloading and cleaning CosIng Annex II and Hugging Face datasets
- Data preprocessing: cleaning and standardizing ingredient names
- Model development: TF-IDF feature extraction and training Logistic Regression for binary classification
- OCR integration: built a pipeline using pytesseract to extract ingredients from images
- Evaluation: generated metric, confusion matrix, and tested edge cases (like substring false positive, etc)
- Report writing: summarizing methodology, performance, and potential extensions
