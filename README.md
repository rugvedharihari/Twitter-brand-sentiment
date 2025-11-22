
⚙️ How It Works

1️⃣ Data Collection  
Tweets were scraped based on smartphone-related keywords and brand names, resulting in a dataset of **12k+ tweets**.

2️⃣ Preprocessing  
Text normalization steps included:
- Lowercasing, cleaning, stopword removal  
- Emoji decoding → `"🔥"` → `"fire"`  
- Hindi phrase translation via Google Translate API  
- Detecting brand mentions using regex patterns

3️⃣ Classical ML (TF-IDF + XGBoost)  
- Converted cleaned text into TF-IDF vectors  
- Trained an XGBoost classifier on manually labeled sentiment data  
- Evaluated accuracy, F1-score, and confusion matrix

4️⃣ BERT Fine-Tuning  
- Loaded pre-trained BERT  
- Fine-tuned on an external sentiment dataset (e.g., Tweets/Reviews dataset)  
- Used the fine-tuned model to predict sentiment on the cleaned smartphone tweets

5️⃣ Insights  
- Compared sentiment distribution across **9 major smartphone brands**  
- Observed differences between XGBoost predictions and BERT predictions  
- Highlighted brand strengths and weaknesses based on public opinion

🏁 Conclusion

This project demonstrates how combining **traditional ML** with **state-of-the-art transformers** can yield strong performance on sentiment classification tasks.  
It also highlights the importance of high-quality preprocessing (emoji decoding, translation, regex extraction) in achieving meaningful insights from noisy social media data.

---

## 📧 Contact

If you'd like to discuss the project, improve the models, or collaborate on NLP/ML work, feel free to reach out!

