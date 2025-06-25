# SentencePiece and Byte-Pair Encoding (BPE) Implementation

## Overview

This repository contains code and explanations demonstrating SentencePiece tokenization and the Byte-Pair Encoding (BPE) algorithm, both fundamental techniques for text encoding in Natural Language Processing (NLP). The goal is to provide a clear understanding of how these methods work, particularly in the context of preparing text data for use with neural network models.

**Note:** The core structure and exercises are adapted from a programming assignment in the **[Natural Language Processing Specialization](https://www.coursera.org/specializations/natural-language-processing)** by DeepLearning.AI.
## Contents

*   **`C4W3_SentencePiece_and_BPE.ipynb`:** A Jupyter Notebook containing the main code and explanations.  It covers:
    *   Introduction to tokenization and its challenges.
    *   SentencePiece preprocessing steps (NFKC normalization, lossless tokenization).
    *   Implementation of the BPE algorithm from scratch.
    *   Training and using the SentencePiece library.
    *   Comparison of the custom BPE implementation with SentencePiece.
*   **`data/`:** Directory containing sample data used in the notebook.  Specifically, `data.txt` is used for demonstration.
    *   `data.txt`: A small dataset of text examples in json format, originally from the Squad dataset.
    *   `sentencepiece.model`: Pre-trained SentencePiece model provided with the course assignment.

## Getting Started

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/mahdertesf/SentencePiece-and-Byte-Pair-Encoding-BPE-Implementation.git
    cd [repository name]
    ```

2.  **Install the required libraries:**

    ```bash
    pip install ast sentencepiece regex
    ```
    If running in a Jupyter Notebook environment make sure the kernel is selected.

3.  **Open and run the Jupyter Notebook .**

    Follow the instructions and explanations within the notebook to understand the code and experiment with SentencePiece and BPE.

## Key Concepts Covered

*   **Tokenization:** Splitting text into meaningful units (tokens).
*   **Subword Tokenization:**  Breaking words into smaller units to handle out-of-vocabulary words and improve model generalization.
*   **Byte-Pair Encoding (BPE):**  A data compression algorithm adapted for subword tokenization, iteratively merging the most frequent pairs of characters or character sequences.
*   **SentencePiece:** A library implementing subword tokenization algorithms, including BPE and Unigram language models.
*   **NFKC Normalization:**  A Unicode normalization form used by SentencePiece to ensure consistent character representation.
*   **Lossless Tokenization:** Preserving whitespace information during tokenization and detokenization.

## Usage

The notebook provides a step-by-step guide to:

*   Preprocessing text data for SentencePiece and BPE.
*   Implementing the BPE algorithm from scratch.
*   Training a SentencePiece BPE model on the provided example data.
*   Encoding and decoding text using the trained SentencePiece model.
*   Comparing the output of the implemented BPE algorithm with the SentencePiece library's BPE implementation.
