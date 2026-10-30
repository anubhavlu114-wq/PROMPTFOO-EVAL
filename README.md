# 🚀 Promptfoo LLM Evaluation & Benchmarking Suite

An automated prompt evaluation and benchmarking workspace built using **Promptfoo** and a custom **Python Provider Interface**. This setup enables systematic testing of prompt iterations, tracking pass/fail rates, execution latency, and custom variable substitutions.

---

## 📌 How Promptfoo Works

Promptfoo is an open-source CLI and library designed to evaluate LLM output quality deterministically. 

1. **Config Definition (`promptfooconfig.yaml`):** Defines prompt templates, variable test cases, assertions, and model providers.
2. **Evaluation Pipeline:** Evaluates each prompt against every variable permutation using the configured provider execution layer.
3. **Matrix Results:** Generates pass/fail metrics, token usage, and latency analysis in a browser dashboard.

---

## 🧪 Evaluated Test Cases & Prompts

Derived from evaluation benchmark runs:

### 1. Evaluated Prompts
* **Baseline Prompt:** `Write a tweet about {{topic}}`
* **Variation Prompt:** `Write a concise, funny tweet about {{topic}}`

### 2. Dynamic Variables
* `bananas`
* `avocado toast`

### 3. Execution Summary
* **Provider:** Custom Python execution script (`python:provider.py:default`)
* **Pass Rate:** 100.00% Passing (2/2 cases)
* **Average Latency:** ~516ms – 517ms

---

## 📂 Repository Layout

```text
.
├── promptfooconfig.yaml    # Core evaluation suite configuration
├── provider.py             # Custom Python provider script / LLM wrapper
├── assets/                 # Evaluation screenshots & visual benchmarks
│   ├── eval_matrix.png     # Web Dashboard results matrix
│   └── terminal_setup.png  # CLI server execution log
├── .gitignore
└── README.md
<img width="1898" height="758" alt="eval_matrix" src="https://github.com/user-attachments/assets/a7e7feb8-5dba-44fb-9d46-082c6d3b80cd" />
<img width="1410" height="783" alt="terminal" src="https://github.com/user-attachments/assets/e12f7bc5-e5e0-42a4-befd-754914124a07" />
