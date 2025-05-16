# Code Alpaca 20K – Code + Explanation

🧠 A dataset designed to enhance large language models (LLMs) with **code generation** and **instructional explanation** capabilities.  
This version is an extension of the original [`sahil2801/CodeAlpaca-20k`](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k), with AI-generated explanations added to the `output` section using the Gemini API.

---

## 📘 Overview

This dataset enhances the original **CodeAlpaca-20k** examples by adding natural language explanations to code outputs.

The goal is not just to generate code, but also to support user learning by explaining the code in an **instructive manner**.

This enables models to go beyond simply solving problems, allowing them to engage in a more **educational and guiding way**.

A model fine-tuned on this dataset is expected to:

- Generate valid code  
- Explain how the code works step-by-step  
- Suggest practical exercises  
- Ask follow-up questions to help reinforce understanding  

---

## 📦 Data Structure

Each data sample consists of the following fields:

| Field         | Description                                       |
|---------------|-------------------------------------------------|
| `instruction` | The prompt or task description                    |
| `input`       | Optional input or context (can be empty)          |
| `output`      | Output containing both the code and its explanation |

> ⚠️ All explanations are generated using the Gemini API and are consistent in tone and structure.

---

## 🔍 Example

```json
{
  "instruction": "Write a Python function that reverses a string.",
  "input": "",
  "output": "def reverse_string(s):\n    return s[::-1]\n\n# Explanation:\n# This function takes a string 's' and uses slicing to return the reversed string. The notation 's[::-1]' is a Python idiom for reversing strings."
}
```
## 📜 License

This dataset inherits the original [`sahil2801/CodeAlpaca-20k`](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k) license: CC BY 4.0. Please ensure compliance with licensing terms when using or distributing

## 👤 About the Author 

Hasan Basri Gedik Passionate about artificial intelligence, machine learning, and deep learning. Loves problem solving, interested in cryptographic algorithms, and an active chess player.

📫 Contact: hasanbgedik@gmail.com

🔗 GitHub: https://github.com/hasan1108
