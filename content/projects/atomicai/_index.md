---
title: Automic Chess AI
toc: false
cascade: 
    type: blog
---

### Introduction

I built AtomicAI, an AI that plays Atomic Chess, a variant of regular chess where captured pieces explode. The goal was to create a deep learning-based evaluation function that rates board positions and helps a chess engine make better moves.

### The Challenge

Unlike standard chess, Atomic Chess has unique tactical patterns, and there is limited domain knowledge available for designing an evaluation function. Traditional engines rely on handcrafted heuristics, but our approach leverages deep learning to learn position strength directly from game data.

### Approach
- Collected 900,000+ games from the Lichess database, filtering only high-level (Elo 2000+) matches to ensure strategic depth. We then extracted 2 million board states for training.
- Designed a CNN-based evaluation function that assesses a given board position and assigns a value between 0 (winning for Black) and 1 (winning for White). The model learns spatial relationships between pieces, making it more adaptable than handcrafted heuristics.
- We integrated our AI with Andoma, a Python-based chess engine, allowing it to play complete games against humans and other AI opponents

### Code
{{< card link="https://github.com/IsmailOuazzani/AtomicAI" title="View on Github" icon="github" >}}

### Project Report
{{< pdf "atomic_ai_report.pdf" >}}