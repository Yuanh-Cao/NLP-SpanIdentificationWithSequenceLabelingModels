# NLP-SpanIdentificationWithSequenceLabelingModels
## Natural Language Processing
### from Cornell University CS4740/5740 2020Fall

Work by Yuanhong Cao (yc2668@cornell.edu), Zeyu Chen (zc436@cornell.edu)

link to raw data: https://drive.google.com/drive/folders/1R7ZI2aZSXEpczLKTF-Zv9i5sfNuse3s4?usp=sharing

In this project, you will implement a model that identifies relevant information in a text and tags it with the appropriate label. Particularly, the task of this project is Propaganda Identification. The given dataset contains (manual) annotations indicating fragments of text that exhibit one of a set of well-known propaganda techniques. Your task is to develop NLP models to identify these propagandistic spans of text automatically. We will treat this as a sequence-tagging task: for each token in the input text, assign a label  𝑦∈{0,1} , such that 1 represents propagandistic text and 0 represents non-propaganda. (A description of the original task formulation is here. We are working on a modified version of their "span identification" task.)

For this project, you will implement two sequence labeling approaches:

Model 1 : a Hidden Markov Model (HMM)
Model 2 : a Maximum Entropy Markov Model (MEMM), which is an adaptation of an HMM in which a Logistic Regression classifier (also known as a MaxEnt classifier) is used to obtain the lexical generation probabilities (i.e., the observation/emission probability matrix, so "observations" == "emissions" == "lexical generations"). Feature engineering is strongly suggested. (Papers from the Workshops on Figurative Language Processing can provide good insights on feature selection for this task.) You can also refer to the J&M book.
