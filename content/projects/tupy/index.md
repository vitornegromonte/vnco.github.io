---
title: "Tupy: A Lightweight Energy Optimization for AI training"
date: 2024-10-26
lastmod: 2024-10-26
tags: ["Python", "Optimization", "PyTorch", "Deep Learning", "Linear Programming"]
author: ["Vitor Negromonte"]
description: "A Lightweight Energy Optimization Package for PyTorch."
summary: "Energy Optimization during AI training"
cover:
  image: "tupy.png"
---

##### Description
**Tupy** is a streamlined package aimed at **optimizing energy consumption** for *PyTorch-based* AI models and, eventually, *TinyGrad*. By tracking and minimizing resource usage during training, Tupy empowers developers and researchers to reduce the carbon footprint of their AI projects without compromising model performance. This tool is ideal for anyone looking to incorporate sustainable practices into their machine learning workflows, especially in resource-constrained environments.

> Tupy comes from *Tupã*, which means "Thunder" in [Tupi](https://en.wikipedia.org/wiki/Tupi_language), the largest indigenous language in Brazil.

---
##### Features
- Real-time energy monitoring
- Real-time optimization of energy consumption
- Support for PyTorch

##### Directory Structure
```bash
tupy/
├── src/
│   ├── __init__.py
│   ├── monitor.py
│   ├── optimizer.py
│   └── callbacks.py
├── tests/
│   ├── __init__.py
│   ├── test_monitor.py
│   ├── test_optimizer.py
│   └── test_callbacks.py
├── docs/
│   └── index.md
├── setup.py
└── README.md
``` 

---
##### Installation
```python
pip install tupy
```

##### More in
+ [GitHub](https://github.com/vitornegromonte/tupy)
+ [Technical report coming soon!]()