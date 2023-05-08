# Smart-Assessment-Tool-For-Descriptive-Answers
Automated evaluation of handwritten subjective exam papers is an important area of research with potential applications in the education sector. The project aimed to develop a system that used OCR technology and string matching algorithms to automate the evaluation of handwritten subjective exam papers, with the objective of reducing the workload of examiners and providing faster and more accurate evaluation.
The proposed methodology involved using OCR technology to convert scanned documents into machine-readable text, followed by keyword extraction and string matching algorithms for evaluation. The system was developed using Python and some libraries, including NLTK and FuzzyWuzzy. The limitations of existing models and algorithms provided the motivation for this project, which aimed to improve the accuracy and efficiency of handwritten subjective exam paper evaluation.
The expected outcome of this project was a system that could automate the evaluation of handwritten subjective exam papers accurately and efficiently. Future work could involve the use of deep learning models, such as Recurrent Neural Networks (RNNs), for further improving the accuracy of the system. Additionally, the system could be extended to evaluate other types of responses, such as flow charts and diagrams.

The evaluator must provide the answer key for the given questions. The handwritten responses of the learner must be scanned and uploaded. The system will convert the handwritten document to text using Optical Character Recognition (OCR). OCR is a technology that converts scanned text images into machine-readable text formats. The process involves-
Preprocessing - remove the background noise, enhance the region of interest in image and make a clear difference between foreground and background. In order to achieve these goals: noise filtering, conversion to binary and smoothing operations are performed on the input image
Feature Extraction - Feature vector is calculated from the processed image.
Text recognition - done by passing the obtained feature vector as input to machine learning algorithms to analyze and recognize the shapes and strokes of handwritten characters.
The model takes an image file as input, which could be a scanned document or a photo of text. The image is preprocessed to enhance its quality and make it easier to recognize the text. This includes operations like thresholding, smoothing, and binarization [1]. The preprocessed image is then passed to OCR engine, which analyzes the image and extracts the text using techniques such as character segmentation, feature extraction, and classification. The recognized text is returned to the Python program. The Python program then processes the recognized text further for evaluation. Extracting keywords from the learner’s  response involves -
Tokenizing text into words.
Counting frequency of each word and identifying keywords based on their frequency.
Removing duplicates from the word list.
Since learners can explain answers in different ways, WordNet will be used to check synonyms, of the keywords from both learner’s response and answer key [5]. The evaluation is done based on four factors namely, similarity factor, keyword factor, grammar factor, keyword accuracy factor. Similarity score is calculated based on fuzzy logic and string matching [2]. Grammar is checked using language_tool_python library. The score is initially set to 0 and is incremented. The detailed report is displayed.
The flowchart for the algorithm followed is shown in Figure 5.1.

![image](https://user-images.githubusercontent.com/119789101/236781611-2c002f67-c6a6-4ac4-88d9-20bedd739672.png)

Figure 5.1 - Algorithm flowchart

The model uses Convolutional Neural Network (CNN) for text detection and a Long Short-Term Memory (LSTM) network for text recognition. The feature vector obtained after feature extraction is fed as input for the LSTM model [1].

Convolutional Neural Network (CNN) - The main idea behind CNNs is to learn local patterns or features from the input image by applying convolutional filters over the input. These filters detect specific visual patterns such as edges, corners, and textures, which are then combined to form higher-level features. The convolutional filters are learned through backpropagation during training, allowing the network to learn the most relevant features for the given task.
