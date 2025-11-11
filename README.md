
# Vibe Matcher Recommendation Prototype

This project demonstrates a semantic vibe-based fashion recommendation system using OpenAI embeddings.
The system allows users to search fashion products by *vibes* such as "cozy cafe autumn", "energetic urban", etc.

---

## Features
- Converts product descriptions into vector embeddings
- Converts user vibe queries into the same embedding space
- Computes cosine similarity to find closest aesthetic matches
- Returns the **top-3 vibe-aligned product recommendations**

---

## How It Works
1. Fashion items are stored with natural-language descriptions
2. Descriptions are embedded using `text-embedding-ada-002`
3. User enters a vibe phrase (e.g., "soft cozy warm fall energy")
4. Embedding similarity → closest matches returned

---

## Notebook
Run the notebook:
`vibe_matcher_recommendation.ipynb`

Set your OpenAI API key before generating embeddings:

```python
import os
os.environ["OPENAI_API_KEY"] = "your_api_key_here"
```

---

## Next Steps
- Integrate Pinecone or FAISS for scalable vector search
- Add image embeddings for visual aesthetic matching
- Expand dataset + cluster vibes

---

## Why AI at Nexora
I’m drawn to how Nexora explores the intersection of style, identity, and intelligent personalization. Fashion isn’t just about utility—it's expressive, contextual, emotional. AI becomes meaningful when it helps people find what *feels like them*, not just what fits a category. I love building systems that listen for mood, tone, and vibe—not just keywords. Nexora’s approach aligns with what excites me: rapid iteration, creativity, and real user impact.

---
