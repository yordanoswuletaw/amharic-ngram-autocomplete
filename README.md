# Amharic N-Gram Language Model for Auto-Complete

This project implements an N-Gram language model for the Amharic language, designed to provide auto-complete functionality. The model uses a simple N-Gram propabilistic model to predict and suggest the most probable next words based on input sequences.

## Features

- **N-Gram Based Predictions**: Supports unigram, bigram, trigram and n-gram models to generate context-aware suggestions.
- **Amharic Language Support**: Handles the structure and highly morphological nature of Amharic text.
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
├── data/                        # Dataset for training, dev and testing
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

## Requirements

- Python 3.8+
- Required Python libraries (see `requirements.txt`)

## Examples

```text
Input: አበበ በሶ
Suggestions: በላ
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

# amharic-ngram-autocomplete
