Price Sentiment Analysis with RoBERTa

This project focuses on sentiment analysis of customer reviews in the pricing domain. The main objective is to classify whether customers perceive the product/service price as positive, neutral, or negative.

Labels

Each review is annotated with a sentiment label related to price perception:

1 → Positive (Fair/Good price)
Example: "The price was excellent and totally worth it."

0 → Neutral (Price not mentioned)
Example: "The product quality is great."

-1 → Negative (Expensive/Unfair price)
Example: "The price was too high for what I got."

Dataset

The dataset contains customer reviews that target the pricing aspect.
It is split into train (80%) and test (20%) sets for training and evaluation.

Model

We fine-tuned RoBERTa (a transformer-based language model) on this dataset.
Framework: Hugging Face Transformers
Training: 10 epochs, batch size 16, weight decay 0.01
Logging and evaluation at each epoch

Results

The fine-tuned RoBERTa model achieved:
Accuracy: ~96%
Strong performance across all three classes (Positive, Not Mentioned, Negative)
This shows that transformer-based models are highly effective for domain-specific sentiment analysis.
