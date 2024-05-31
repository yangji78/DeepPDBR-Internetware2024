# DeepPDBR: Internetware 2024 Artifact

***

ICSE 2020 Artifact for: `Predicting Docker Build Result based on Deep Abstract Syntax Tree and Deep Neural Network`.

## Reproducing experimental results

***

### AST parse

1. Run `./experiments/I-parse/1-phase-1-dockerfile-asts/generate.sh` for parsing phase I.
2. Run `./experiments/I-parse/2-phase-2-dockerfile-asts/generate.sh` for parsing phase II.
3. Run `./experiments/I-parse/3-phase-3-dockerfile-asts/generate.sh` for parsing phase III.
4. Run `./experiments/I-parse/4-phase-4-dockerfile-asts/generate.sh` for parsing phase IV.

### Feature extract

1. Run `./experiments/II-feature/word2vec` for corpus training.
2. Run `./experiments/II-feature/feature_save` for feature saving.

### Results prediction

1. Run `./experiments/III-prediction/icpads_predict.py` for prediction prediction.
2. Run `./experiments/III-prediction/pretrained_predict.py` for BERT models prediction.
3. Run `./experiments/III-prediction/rnn_predict.py` for GRU/LSTM prediction.
4. Run `./experiments/III-prediction/transformer_predict.py` for DeepPDBR (**Our Method**) prediction.

#### RQ6.2 Incorrect predictions analysis

For this part of the discussion, we selected 100 Dockerfile prefix names as shown in RQ6.2-IDs.csv.