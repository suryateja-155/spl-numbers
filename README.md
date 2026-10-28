<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0C4A6E,0284C7,38BDF8&height=220&section=header&text=Special%20Number%20Range%20Filter&fontSize=40&fontColor=ffffff&fontAlignY=38&desc=Interval-Based%20Mathematical%20Search%20and%20Range%20Optimization&descSize=16&descAlignY=60&descAlign=50" width="100%" alt="Special Number Range Filter Banner"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Language-Python%203.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Language Python 3.10+"/>
  <img src="https://img.shields.io/badge/Domain-Interval%20Computing-0284C7?style=for-the-badge" alt="Domain Interval Computing"/>
  <img src="https://img.shields.io/badge/Optimization-Range%20Pruning-38BDF8?style=for-the-badge" alt="Optimization Range Pruning"/>
  <img src="https://img.shields.io/badge/License-MIT-7DD3FC?style=for-the-badge" alt="License MIT"/>
</p>

---

## Executive Summary / Overview
### Problem Statement & Context
While verifying a single special number is straightforward, scanning an expansive numerical interval [A, B] requires minimizing redundant calculations and applying early-exit pruning to avoid unneeded factorial evaluations.

### Solution Overview
This repository implements a **Range-Based Special Number Filter** in Python. The implementation sweeps across arbitrary intervals, filtering and aggregating numbers whose digit-factorial sum strictly matches their identity.

---

## Interactive Table of Contents
- [Executive Summary / Overview](#executive-summary--overview)
- [Key Features & Capabilities](#key-features--capabilities)
- [System Architecture / Pipeline](#system-architecture--pipeline)
- [Tech Stack Breakdown](#tech-stack-breakdown)
- [Reproducible Quickstart & Setup](#reproducible-quickstart--setup)
- [Project Directory Layout](#project-directory-layout)
- [Author & Contributions](#author--contributions)

---

## Key Features & Capabilities
- **Bounded Interval Search:** Iterates through user-defined lower and upper bounds [A, B].
- **Modular Function Isolation:** Decouples the single-number verification predicate from the interval scanning engine.
- **Result Aggregation:** Accumulates discovered special numbers into clean Python lists for further analysis.

---

## System Architecture / Pipeline
```mermaid
flowchart TD
    Bounds["Input Range: [Start, End]"] --> Generator[Range Iterator]
    Generator --> Predicate{Is Special Number?}
    Predicate -- True --> Append[Append to Results List]
    Predicate -- False --> Next[Skip / Next Iteration]
    Append --> Next
    Next --> Done{Range Exhausted?}
    Done -- No --> Generator
    Done -- Yes --> Output[Return Matching Special Numbers]
```

---

## Tech Stack Breakdown
| Layer | Technology | Role |
| :--- | :--- | :--- |
| **Languages** | Python 3.10+ | Standard mathematical expressions and loops |
| **Libraries** | Python Standard Library | Integer range generators and list collections |
| **Tools** | Jupyter Notebook | Stepwise evaluation and demonstration |
| **Architecture** | Interval Filter Pipeline | Bounded range iteration with predicate validation |

---

## Reproducible Quickstart & Setup
```bash
# 1. Clone repository
git clone https://github.com/suryateja-155/spl-numbers.git
cd spl-numbers

# 2. Run notebook
jupyter notebook "speacial numbers between the range.ipynb"
```

---

## Project Directory Layout
```text
spl-numbers/
├── speacial numbers between the range.ipynb # Range filtering and search logic
└── README.md                                # Algorithmic optimization guide
```

---

## Author & Contributions

**Gettupalli Surya Teja**  
- GitHub Profile: [@suryateja-155](https://github.com/suryateja-155)  
- Portfolio Index: [Gettupalli-Surya-Teja](https://github.com/suryateja-155/Gettupalli-Surya-Teja)

Contributions, issue reports, and feedback are always welcome! Feel free to open an issue or pull request.

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0C4A6E,0284C7,38BDF8&height=100&section=footer" width="100%" alt="Footer Banner"/>
</p>
