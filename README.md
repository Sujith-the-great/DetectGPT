# Detect-GPT: Zero-Shot AI-Generated Text Detection
This repository contains the implementation and analysis of Detect-GPT, a zero-shot AI-generated text detection model. The project explores using the curvature of the log probability function to distinguish between human-written and AI-generated text without the need for pre-existing training data.

## Project Overview
As large language models (LLMs) become more sophisticated, identifying AI-generated text presents a growing challenge. Detect-GPT leverages the behavior of LLMs in probability space, where AI-generated text typically resides near local maxima in the log probability function, characterized by negative curvature. This project enhances the understanding of Detect-GPT’s performance and proposes modifications to its hypothesis and methodology.

## Key Features
**Zero-Shot Detection**: No training data required for text classification.


**Log Probability Curvature**: Identifies AI-generated text by analyzing the log probability of perturbed text samples.

**Transformer-Based Models**: Utilizes models like GPT-2 and T5-small for source text generation and perturbations.

**Comprehensive Experiments**: Evaluates performance on datasets such as Multi-News, XSum, PubMedQA, WMT16, and SQuAD.

## Implementation Highlights
**Model Architecture**: Uses the log probability function of transformer models to classify text as human-written or AI-generated.
**Perturbation Analysis**: Introduces controlled modifications to text and analyzes discrepancies in log probabilities.
**ROC and Precision-Recall Evaluation**: Assesses model performance across datasets with detailed metrics.
**Hypothesis Modification**: Explores alternative approaches to enhance the accuracy of human-written text classification.
## Results
The experiments reveal the potential and limitations of Detect-GPT, showing its strengths in detecting AI-generated text while identifying areas for improvement, such as hyperparameter tuning and model scope.

## Future Work
Optimize hyperparameters and explore advanced perturbation techniques.
Experiment with larger and more diverse datasets.
Enhance model performance by refining scoring mechanisms and decoder prompts.
