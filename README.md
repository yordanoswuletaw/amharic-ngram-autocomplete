# Amharic N-Gram Language Model for Auto-Complete

This project implements an N-Gram language model for the Amharic language, designed to provide auto-complete functionality. The model uses a simple N-Gram propabilistic model to predict and suggest the most probable next words based on input sequences.

## Features

- **N-Gram Based Predictions**: Supports unigram, bigram, trigram and n-gram models to generate context-aware suggestions.
- **Amharic Language Support**: Handles the unique structure and highly morphological nature of Amharic text.
- **Tokenization**: Includes an Amharic-specific tokenizer to handle words and punctuation correctly.
- **Smoothing Techniques**: Implements smoothing methods (e.g., Laplace smoothing) to address the issue of zero probabilities.
- **Scalable Design**: Can be trained on large datasets for improved accuracy.

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yordanoswuletaw/amharic-ngram-autocomplete.git
   ```
2. Navigate to the project directory:
   ```bash
   cd amharic-ngram-autocomplete
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Training the Model

1. Prepare your Amharic text corpus and place it in the `data/` directory.
2. Run the training script:
   ```bash
   python train.py --corpus data/corpus.txt --ngram_size 3
   ```
   Replace `--ngram_size` with `1`, `2`, or `3` to specify the N-Gram size.

### Using the Auto-Complete

1. Start the auto-complete interface:
   ```bash
   python autocomplete.py
   ```
2. Type an input phrase in Amharic, and the model will suggest the most likely completions.

Example:
```text
Input: አበበ በሶ
Suggestions: በላ
```

---

## Repository Structure

```plaintext
├── .vscode/
│   └── settings.json            # VS Code settings for environment setup
├── .github/
│   └── workflows/
│       ├── unittests.yml        # CI/CD pipeline for unit tests
├── .gitignore                   # Ignored files and folders
├── requirements.txt             # Dependencies for the project
├── README.md                    # Documentation of the repository
├── src/                         # Source code for analysis and processing
├── notebooks/
│   ├── __init__.py              # Package initialization
│   └── README.md                # Documentation for the notebooks
├── tests/
│   ├── __init__.py              # Test initialization
└── scripts/
    ├── __init__.py              # Scripts package initialization
    └── README.md                # Documentation for scripts
```

---

## Requirements

- Python 3.8+
- Required Python libraries (see `requirements.txt`)

## Examples

```text
Input: ከልላዕ
Suggestions: ከልላገ ከልላም ከልላስ
```

## Future Work

- Integrate neural language models for amharic langauge tokenization.
- Expand support for additional Amharic linguistic features and dialects.

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue to suggest improvements or report bugs.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

Special thanks to:
- The Amharic NLP community for providing open-source datasets.
- Researchers and contributors to N-Gram language modeling techniques.

---
# amharic-ngram-autocomplete
