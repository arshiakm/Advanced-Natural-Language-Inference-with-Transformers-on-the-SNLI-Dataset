# Advanced Natural Language Inference with Transformers on the SNLI Dataset

This repository hosts the implementation of the project **"Enhancing the Accuracy and Robustness of Natural Language Inference Models Using Advanced Techniques on the SNLI Dataset"**. This project aims to improve Natural Language Inference (NLI) model performance using advanced transformer architectures and innovative training methods, achieving state-of-the-art results on the SNLI dataset.

## Project Overview
Natural Language Inference (NLI) is a core task in natural language processing (NLP) where the goal is to determine the relationship between two sentences: the **premise** and the **hypothesis**. This project evaluates popular transformer-based architectures, such as BERT, RoBERTa, and DeBERTa, and introduces advanced training strategies to improve their accuracy and robustness. The **DeBERTa** model achieved the best results, with a test accuracy of **91.78%**.

### Key Highlights:
- Comprehensive evaluation of leading transformer-based models.
- Implementation of advanced training techniques, including mixed precision training, gradient accumulation, and regularization.
- Data augmentation methods like synonym replacement and back-translation to enhance data variability.
- Extensive error analysis and performance visualizations.

## Dataset
The [Stanford Natural Language Inference (SNLI) dataset](https://nlp.stanford.edu/projects/snli/) is used, comprising over **570,000 human-labeled sentence pairs** categorized as:
- **Entailment**
- **Contradiction**
- **Neutral**

Preprocessing steps ensure tokenization, balanced label distribution, and efficient data handling.

## Models and Training Strategies
### Models:
- **BERT**: Achieved 86.69% test accuracy.
- **RoBERTa**: Achieved 89.67% test accuracy.
- **DeBERTa**: Best-performing model with 91.78% test accuracy.

### Advanced Techniques:
- **Mixed Precision Training**: Improved computational efficiency and reduced memory usage.
- **Gradient Accumulation**: Enabled training with larger effective batch sizes on memory-limited devices.
- **Regularization**: Prevented overfitting using dropout and weight decay.
- **Model Ensembling**: Combined predictions from multiple models for higher accuracy.

## Results
| Model            | Validation Accuracy | Test Accuracy |
|-------------------|---------------------|---------------|
| Transformer-base  | 68.10%             | 67.86%        |
| BERT             | 86.56%             | 86.69%        |
| RoBERTa          | 89.82%             | 89.67%        |
| DeBERTa          | **91.24%**         | **91.78%**    |

DeBERTa's advanced architecture, incorporating disentangled attention mechanisms and enhanced embeddings, enabled it to capture complex linguistic relationships effectively.

## Getting Started
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/advanced-nli-transformers.git
   cd advanced-nli-transformers
