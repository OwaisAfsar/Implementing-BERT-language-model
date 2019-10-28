# Implementing-BERT-language-model
Implementing BERT language model on OffensEval dataset

BERT stands for 'Bidirectional Encoder Representations from Transformers'. BERT is designed to pretrain deep bidirectional representations 
from unlabeled text by jointly conditioning on both left and right context in all layers. As a result, the pre-trained BERT model can be 
finetuned with just one additional output layer to create state-of-the-art models for a wide range of tasks, such as question answering and
language inference, without substantial taskspecific architecture modifications.

## Point for running the code:##
* Make sure to add dataset files in 'Dataset' forlder.
* After training the model, 3-files will be generated in Output folder. 
### For testing purpose:###
* Go into the outputs/'Name' directory where the fine tuned models will be saved. There, you should find 3 files; config.json, 
  pytorch_model.bin, vocab.txt.
* Archive the two files (I use 7zip for archiving) config.json, and pytorch_model.bin into a .tar file.
* Compress the .tar file into gzip format. Now the file should be something like yelp.tar.gz
* Copy the compressed file into the cache/ directory. i.e. We will load this fine tuned model in the next step.
* The result will be save in reports folder in .txt format.
