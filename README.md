# Disinformation-Detection-with-LLMs-Dataset
This repository contains the dataset used in the article: “Disinformation detection with LLMs: Can different models agree on their judgment?”

# Disinformation Detection with LLMs: Dataset

This repository contains the dataset used in the article:  
**“Disinformation detection with LLMs: Can different models agree on their judgment?”**

Dataset was annotated by fact-checking and debunking experts using methodology created by these experts in colaboration with researchers. 
This repository contains the **annotations and evaluations performed by LLMs (Gemini, LLaMA 405, GPT-3.5)** on top of that high-quality human annotated data.

The dataset includes news and opinion articles annotated by different large language models (LLMs). Each model provides its judgment on whether the article constitutes **reliable information** or **disinformation**, along with reasoning, identified manipulation techniques, and key points.

---

## 📂 Dataset Structure

The dataset is provided in CSV format. Each row corresponds to one article.  

### Columns
- **article_id** – Unique identifier for each article.  
- **article_title** – Title of the article.  
- **article_text** – Full text of the article  
- **topic** – Main topic of the article  
- **article_credibility_assessment_type** – Ground truth label assigned during dataset preparation (*disinformation / reliable_information*).  
- **manipulation_type** – Detected manipulation methods (e.g., *CHERRY_PICKING, EXAGGERATION, FALSE_CAUSE*).  

For each LLM (Gemini, LLaMA 405, GPT-3.5), the following fields are available:  
- **base_prompt_[MODEL]** – The model’s direct classification (*disinformation / reliable_information*).  
- **reason_disinformation_base_[MODEL]** – Explanation provided by the model.  
- **verdict_[MODEL]** – Final decision of the model.  
- **key_points_[MODEL]** – Main arguments or signals identified by the model.  
- **categories_[MODEL]** – Themes  assigned to each model derived from the key points using thematic analysis.
---


## 🔍 Research Context
This the data were used to investigate the potential of Large Language Models (LLMs) as disinformation detectors, examining how these models perceive and evaluate disinformation.
Reserch questions are the following: 
1. To what extent LLMs can be used to detect disinformation.  
2. The key characteristics in text that influence LLMs’ credibility judgments.  
3. Whether different models (Gemini, LLaMA, GPT) converge or diverge in their classifications.  

---

## 📑 Citation

If you use this dataset, please cite our article:  
> [Full citation to be added after publication]

---

## ⚖️ License

Note: The original data was collected by colleagues in other research projects and is reused here with permission.  
This dataset is released under the **CC0 1.0 Universal License**. Please check the `LICENSE` file for details.  
