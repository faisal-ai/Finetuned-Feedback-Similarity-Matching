# Feedback–Backlog Similarity Matching

This project aims to match free-text user feedback with product backlog items using modern NLP techniques. The goal is to help product and engineering teams triage feedback at scale and prioritize roadmap items based on actual user needs.

---

## Project Highlights

- Fine-tuning `Sentence-BERT` using **manually labeled feedback–backlog pairs**.
- Embedding-based retrieval using **FAISS** for scalable similarity search.
- (Optional) Re-ranking with **CrossEncoder** models for higher precision.
- Ready for integration with product feedback systems or issue triage pipelines.

---

## Dataset

The training data consists of feedback–backlog pairs with similarity labels:

```csv
feedback_text,backlog_text,label
"App crashes after update","Fix crash on app startup after update",1
"Dark mode broken","Correct color contrast issues in dark mode",1
"User can't login","Add password strength meter",0
...
