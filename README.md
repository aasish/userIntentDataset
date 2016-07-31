# User Intent Prediction Datset
The goal is to let intelligent agents interpret and learn high-level user intents which span multiple mobile apps, e.g., to plan a dinner we may need to use Yelp, Maps, SMS, etc.

# Contents

## App Descriptions provided by Google Play

## Constructed Graphs

## Graph Labeling Output

## Embedding Vectors

## Seed Cluster Distribution


## App Sequence Data
In sequence_labeling directory you will find following:
1. train, test, dev splits for app sequences `train.apps.int`, `test.apps.int`, `dev.apps.int`. The numeric ids correspond to labels provided `apps.csv` file. 
2. B/I/O tagging information for the app sequences `train.labels.int`, `test.labels.int`, `dev.labels.int`. The numeric ids correspond to labels provided in `labels.csv` file.
3. CRFSuite sequence labeling models for these sequences. 

# Resources
1. App invocation sequences collected from 19 users' Android phones (`R1.csv`);
2. Clean app sequences (apps irrelevant to the intents removed) with user intents annotated by participants (`R2.csv`);
3. Speech commands (both manual transcripts and Google ASR 1-best hypotheses) at app level to re-enact part of intents in 2 (`R3.csv`).

# License
Creative Commons License 1.0 
# Contact
For any questions/suggestions contact: mings@cs.cmu.edu, aasishp@gmail.com
