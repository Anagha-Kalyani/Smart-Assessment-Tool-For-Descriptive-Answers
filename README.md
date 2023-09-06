# Smart Assessment Tool for Descriptive Answers

## Introduction

Automated evaluation of handwritten subjective exam papers is an important research area with significant potential applications in the education sector. This project aims to develop a system that utilizes Optical Character Recognition (OCR) technology and string matching algorithms to automate the evaluation of handwritten subjective exam papers. The primary objective is to reduce the workload of examiners and provide faster and more accurate evaluation results.

## Methodology

The proposed methodology involves several key steps:

1. **OCR Technology**: The system employs OCR technology to convert scanned handwritten documents into machine-readable text. This process includes preprocessing to remove background noise, enhance the region of interest, and distinguish between foreground and background.

2. **Feature Extraction**: After preprocessing, a feature vector is calculated from the processed image.

3. **Text Recognition**: Machine learning algorithms are utilized to analyze and recognize the shapes and strokes of handwritten characters. The obtained feature vector is used as input for text recognition.

4. **Keyword Extraction**: Once the text is recognized, the system tokenizes it into words and counts the frequency of each word. Keywords are identified based on their frequency, and duplicate words are removed.

5. **Synonym Check**: To account for variations in how learners explain answers, WordNet is used to check synonyms of keywords from both the learner's response and the answer key.

6. **Evaluation Factors**: The evaluation process is based on four factors:
    - **Similarity Factor**: Calculated using fuzzy logic and string matching techniques.
    - **Keyword Factor**: Based on the presence and frequency of keywords.
    - **Grammar Factor**: Checked using the language_tool_python library.
    - **Keyword Accuracy Factor**: Evaluates the accuracy of identified keywords.

## Expected Outcome

The expected outcome of this project is a system capable of automating the evaluation of handwritten subjective exam papers accurately and efficiently. It aims to provide a detailed report of the evaluation results, taking into consideration the factors mentioned above.

## Future Work

Future work could involve the following:

- **Deep Learning Models**: Incorporating deep learning models, such as Recurrent Neural Networks (RNNs), to further enhance the accuracy of the system.

- **Expanding Evaluation Scope**: Extending the system's capabilities to evaluate other types of responses, such as flow charts and diagrams.

## Usage

To use the Smart Assessment Tool for Descriptive Answers:

1. Provide the answer key for the given questions.
2. Scan and upload the handwritten responses of the learners.
3. The system will convert the handwritten documents to text using OCR technology and proceed with the evaluation process.

## Flowchart

The following flowchart illustrates the algorithmic process:

![image](https://user-images.githubusercontent.com/119789101/236781611-2c002f67-c6a6-4ac4-88d9-20bedd739672.png)

## Acknowledgments

This project makes use of various libraries and technologies, including NLTK, FuzzyWuzzy, and language_tool_python, to achieve its objectives. Special thanks to the contributors and developers of these tools.

