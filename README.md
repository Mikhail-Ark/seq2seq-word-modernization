### Using seq2seq models in the task of language modernization
(generation of the modern form of a word from its ancient form)

The project aims to evaluate the possibility of using seq2seq architectures to solve the problem of language modernization.

Because it was not possible to find one-word translations of words from Old Russian into Russian in their original form suitable for solving the problem in open sources, it was necessary to collect and prepare data. Data from free sources are ancient words with associated dictionary entries. The paper assumes that using word2vec, you can get some one-word correspondence for each ancient word. Some of these correspondences will be a true modernized version of the ancient one.

At the next stage, it was necessary to conduct experiments with the architecture of neural networks and configure hyperparameters for the best result. It is assumed that the char-level seq2seq model will be quite effective in solving the problem of language modernization; in particular, it is expected that a bidirectional LSTM with attention will show the best result.

The third stage was to test the generalizing ability of the entire pipeline using the example of English and Old English.
