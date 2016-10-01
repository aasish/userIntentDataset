# User Intent Prediction Datset
The goal is to let intelligent agents interpret and learn high-level user intents which span multiple mobile apps, e.g., to plan a dinner we may need to use Yelp -> Maps -> SMS, etc.

# Contents

## App2Vec
There are several ways to train app embeddings.
You can use doc2vec on app descriptions to project each app into a semantic space. Alternatively, you can collect stream of app invocations from people's smart phones and treat it as a corpus of words and apply word2vec.

## App Sequence Data
In sequence_labeling directory you will find following:
1. train, test, dev splits for app sequences `train.apps.int`, `test.apps.int`, `dev.apps.int`. The numeric ids correspond to labels provided `apps.csv` file. 
2. B/I/O tagging information for the app sequences `train.labels.int`, `test.labels.int`, `dev.labels.int`. The numeric ids correspond to labels provided in `labels.csv` file.
3. CRFSuite sequence labeling models for these sequences. 

# Resources
1. App invocation sequences collected from 19 users' Android phones (`R1.csv`);
2. Clean app sequences (apps irrelevant to the intents removed) with user intents annotated by participants (`R2.csv`);
3. Speech commands (both manual transcripts and Google ASR 1-best hypotheses) at app level to re-enact part of intents in 2 (`R3.csv`).

Feel free to use this dataset. Please consider citing our papers:
### Data Collection
Ming Sun, Yun-Nung Chen, Zhenhao Hua, Yulian Tamres-Rudnicky, Arnab Dash, and Alexander I. Rudnicky, "AppDialogue: Multi-App Dialogues for Intelligent Assistants," in Proceedings of The 10th International Conference on Language Resources and Evaluation (LREC), 2016.
### Application
Ming Sun, Aasish Pappu, Yun-Nung Chen and Alexander I. Rudnicky, "Weakly Supervised User Intent Detection for Multi-Domain Dialogues," in Proceedings of IEEE Workshop on Spoken Language Technology, 2016 (in press).

You can find other research work on this dataset here: http://appdialogue.com/
You can also find a video demo here: https://youtu.be/FvQto8pP1OU

# License
Creative Commons License 1.0 
# Contact
For any questions/suggestions contact: mings@cs.cmu.edu, aasishp@gmail.com
