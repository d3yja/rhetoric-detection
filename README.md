# 🪶 Automating Rhetoric: AI‑Driven Annotation of Early Iberian Women’s Texts

This project explores how Artificial Intelligence can be used to automatically annotate rhetorical devices in historical texts written by 15th-century Iberian women from Castilla-León and Aragón. By combining Large Language Models (LLMs) and traditional NLP methods, we aim to support scholars in analyzing early women's literature at scale.

An article about this can be found here: https://mehtaplus.medium.com/automating-rhetoric-ai-driven-annotation-of-early-iberian-womens-texts-361c759322bb
---

## 📌 Problem Statement

Manual annotation of rhetorical features—like *captatio benevolentiae*, *ethos*, *pathos*, and *allegory*—is time-consuming and requires domain expertise. With the increasing availability of digitized historical corpora, the need for scalable, intelligent annotation tools has grown.

Our goal: Build an AI-assisted pipeline that identifies rhetorical strategies in early Iberian women's texts using both supervised learning (BERT) and few-shot prompting (LLMs like Gemini).

---

## ⚙️ Methods

### 🧠 BERT Fine-Tuning (Supervised Learning)
- Multilingual BERT trained on XML-annotated corpus (converted into token-level CSVs)
- Data preprocessing involved restructuring sentence splits and filtering irrelevant tags
- Outcome: Model failed due to class imbalance and insufficient data

### 💬 Few-Shot Learning with Gemini (LLM)
- Google’s Agent Development Kit used to build an LLM-powered agent
- Prompt included examples + definitions of rhetorical devices
- Asking the model to “explain its decisions” improved accuracy
- Output generated in JSON format for easier interpretation
- PDF upload support added for full-document analysis

---

## 📈 Results

| Method        | Outcome |
|---------------|---------|
| BERT          | Poor performance due to lack of balanced, sufficient training data |
| Gemini LLM    | Reliable identification of rhetorical devices, though some outputs were overly broad or included false positives |

---

