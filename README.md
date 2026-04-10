# ConflictQA

This repository provides the dataset for the paper:

**Exploring Knowledge Conflicts for Faithful LLM Reasoning: Benchmark and Method**

---

## Overview

**ConflictQA** is a benchmark for studying faithful reasoning in large language models under multi-source knowledge conflicts.

---

## Dataset Structure

```text
data/
├── COMP/
│   ├── TextConf/
│   │   ├── Comp_TriplePos.json
│   │   └── Comp_TriplePos_TextConf.json
│   └── TripleConf/
│       ├── Comp_TextPos.json
│       └── Comp_TextPos_TripleConf.json
└── Non-COMP/
    ├── Non_Comp_Pos.json
    ├── Non_Comp_TextConf.json
    └── Non_Comp_TripleConf.json

The dataset is organized into two settings: `COMP` and `Non-COMP`, referring to the **complementary** and **non-complementary** settings, respectively. 
The suffix `_Pos` denotes **positive reasoning scenarios**. 
The suffixes `_TextConf` and `_TripleConf` indicate two types of conflicting evidence: `_TextConf` refers to inconsistency in the **textual evidence**, 
while `_TripleConf` refers to inconsistency in the **KG evidence**. In both cases, such inconsistencies ultimately lead to incorrect answers.

---

## Dataset Structure

This work has been accepted at **SIGIR 2026**.