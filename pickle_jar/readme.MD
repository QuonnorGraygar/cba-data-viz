### Pickle Jar of Pickle Files

This folder contains the pickle files that are used as part of the 
gradient boosting machine for automatic qualitative coding.

There are two kinds of files stored in this folder:
- `q{number}_token_dict.pkl`: stores frequency dictionaries that are used to build the vectors fed into the gradient boosting machine.
- `model_{code}{number}.pkl`: stores gradient boosting machine parameters and hyper-parameters. Models are identified by the code that they assign and the question number that they handle.
