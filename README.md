# glue-benchmark
take on how close we can get to a flexible glue-benchmark where it matters.

## Why
Apart from measuring the progress of research in NLP and NLP transfer learning, the Glue collection offers a good and varied set of low level NLP capabilities which can be used in a variety of higher level solutions. For instance, in large text & news corpora discerning entailment is key to reducing the volume of inputs as well as identifying truly new information.


## Glue Tasks

| Index | Description | Inputs | Target | Metric | SOTA | Huggingface | Best here |
|----|----|----|----|----|----|----|----|
|CoLA | Linguistic acceptability | Sent1 | Binary | Matthews Correlation | |49% | 48% |
| SST-2 | Sentiment analysis | Sent1 | Binary | Accuracy | |92% | 91% |
| MRPC | Sentence equivalence | Sent1, Sent2 | Binary | Accuracy | | 87% | 80% |
| STS-B | Meaning similarity | Sent1, Sent2 | Regression | Correlation | | |
| QQP | Quora Question Pairs, Question equivalence (binary) | Sent1, Sent2 | Binary | Accuracy | |88% | 86% |
| MNLI-m | Matched-Textual entailment (meaning of one fragment is contained in another). Targets: entailment (repeat meaning), contradiction (opposite meaning), or neutral (not relevant) | Sent1, Sent2 | entailment, contradiction, or neutral | Accuracy, F1 | | | |
| MNLI-mm | Same as above, Mismatched- refers to mismatch between trained domains and test domains | Sent1, Sent2 | entailment, contradiction, or neutral | Accuracy, F1 | | | |
| QNLI | Stanford Question Answering Dataset (SQuAD), determine what is the answer and if the answer is available in the paragraph reference | Question, Paragraph | Binary & Sequence with the answer | Accuracy | | 89% | 83% |
| RTE | Recognising Textual Entailment | Sent1, Sent2 | entailment, contradiction, or neutral | Accuracy, F1 | | 71.4% | 54% |
| WNLI | Winograd Schema, Pronoun ambiguity where the answer requires world knowledge and not only grammatical context | Sent1, Sent2 | entailment, contradiction, or neutral | Accuracy, F1 | | 43.7% | 56% |
| AX | DiagnosticMain, Different entailment relationships of arbitrary size predominantly for diagnostic purposes | Sent1, Sent2 | entailment, contradiction, or neutral | Accuracy, F1 | | |  . |

Some of the above are not necessarily relevant

Source: [gluebenchmark.com](https://gluebenchmark.com)
