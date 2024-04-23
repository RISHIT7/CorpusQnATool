# Corpus QnA Tool

Welcome to the Corpus QnA Tool! This project leverages the power of ChatGPT to provide answers to questions based on a custom input corpus. The tool allows you to input a query and receive relevant answers using the provided corpus for context.

## Table of Contents
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)

## Overview
The Corpus QnA Tool is designed to answer user queries based on a specified input corpus. By utilizing ChatGPT, the tool offers intelligent and context-aware responses to your questions. This tool is ideal for projects that require customized QnA capabilities using specific datasets or documents.

## Project Structure
The project is organized as follows:

```
.
├── Corpus
│   ├── Book_1.txt                    # Input corpus for answering queries
│   ├── Book_2.txt                
|   ├──    ...    
|   └── Book_n.txt
├── results
│   ├── paragraph_1.txt               # Most relevant paragraphs
|   ├──    ...
|   ├── paragraph_7.txt
|   └── query.txt                     # Input query
├── .gitignore                        # to Ignore certain files
├── api_call.py                       # To call the chatGPT api
├── Makefile
├── Node.cpp
├── Node.h
├── qna_tool.cpp
├── qna_tool.h
├── tester.cpp
└── README.md                         # Project README
```

- **Corpus**: Contains the input corpus used for answering queries.
- **README.md**: This file provides an overview and guide to the project.
- **requirements.txt**: Lists the Python packages required for the project.

## Installation
To install the required dependencies, run the following command in your terminal:

```bash
pip install -r requirements.txt
```

## Usage
1. **Prepare the Corpus**: Place your input corpus file in the `Corpus` directory. Ensure the file is in a text format and has a file name Book_1.txt, and that the numbers are squential (e.g., `Book_1.txt`, `Book_2.txt`, `...`).

2. **Run the make file**: Run the make file with your chatGPT API_KEY as
```bash
make API_KEY=key
```

3. **Ask Questions**: Once the QnA tool is running, you can input a query and receive an answer based on the provided corpus.

## Customization
You can customize the tool by modifying the source code. For example, you can adjust the response format, specify additional options for ChatGPT, or add support for other types of input corpora.

## Contributing
Contributions are welcome! Please follow the [contribution guidelines](CONTRIBUTING.md) when submitting pull requests or issues.

## License
This project is licensed under the [MIT License](LICENSE). Please see the LICENSE file for more details.
