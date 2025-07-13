# 🤖 Eksplorasi Natural Language Processing dengan Hugging Face Transformers

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg?style=flat&logo=python)
![Transformers](https://img.shields.io/badge/🤗%20Transformers-4.0+-orange.svg?style=flat)
![PyTorch](https://img.shields.io/badge/PyTorch-1.9+-red.svg?style=flat&logo=pytorch)



</div>

---

## 👨‍💻 Profil

**Nama:** Ahmad Fadli Hutasuhut  

---



### 🏆 **Hasil Latihan Praktik (Let's Practice)**

#### **Exercise 1: Sentiment Analysis Comparison**

**Tweet Analysis - Twitter RoBERTa vs Standard Model:**

**Input:** "Artificial intelligence and automation are already causing friction in the workforce. Should schools revamp existing programs for topics like #AI, or are new research areas required?"

**Twitter RoBERTa Model:**
```json
[{'label': 'LABEL_1', 'score': 0.5272255539894104}]
```
*LABEL_1 = Neutral*

**Standard Model:**
```json
[{'label': 'NEGATIVE', 'score': 0.9989722967147827}]
```

**Insight:** Model khusus Twitter mengklasifikasikan sebagai neutral (52.72%), sedangkan model umum melihatnya sebagai negatif (99.90%). Ini menunjukkan pentingnya domain-specific models.

#### **Exercise 2: Topic Classification**

**Input:** "I love travelling and learning new cultures"

**Output:**
```json
{
  "labels": ["travel", "education", "art"],
  "scores": [0.9902299642562866, 0.005778172984719276, 0.003991858102381229]
}
```

**Insight:** Model BART dengan yakin mengklasifikasikan ke kategori "travel" (99.02%), menunjukkan akurasi tinggi dalam zero-shot classification.

#### **Exercise 3: Text Generation**

**Input:** "Hello, I'm a language model"

**Output:** Multiple creative continuations showcasing GPT-2's text generation capabilities.

#### **Exercise 4: Named Entity Recognition**

**Input:** "Her name is Anjela and she lives in Seoul."

**Output:**
```json
[
  {'entity_group': 'PER', 'score': 0.9986631, 'word': 'Anjela'},
  {'entity_group': 'LOC', 'score': 0.9992236, 'word': 'Seoul'}
]
```

**Insight:** BERT berhasil mengidentifikasi person (99.87%) dan location (99.92%) dengan akurasi sangat tinggi.

#### **Exercise 5: Question Answering**

**Input:** 
- **Question:** "Which lake is one of the five Great Lakes of North America?"
- **Context:** "Lake Ontario is one of the five Great Lakes of North America..."

**Output:**
```json
{"score": 0.9834363460540771, "answer": "Lake Ontario"}
```

**Insight:** Model berhasil mengekstrak jawaban yang tepat dengan confidence score sangat tinggi (98.34%).

#### **Exercise 6: Text Summarization**

**Input:** Paragraf tentang Lake Superior

**Output:**
```json
[{"summary_text": "Lake Superior is the largest freshwater lake in the world by surface area. It holds 10% of the world's surface fresh water..."}]
```

**Insight:** Model DistilBART efektif dalam mengompres informasi sambil mempertahankan fakta-fakta kunci.

#### **Exercise 7: Translation**

**Input:** "New York is my favourite city"

**Output:**
```json
[{'translation_text': 'New York ist meine Lieblingsstadt'}]
```

**Insight:** Model T5 berhasil menerjemahkan dari English ke German dengan struktur grammar yang benar.

---
