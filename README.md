# MusicTransformer
Music Transformer - project for AI

## Training
Training is done using sliding sequences, as in the tutorial.

- Given a sequence <A, B, C, D>, input sequence is <A, B, C>, target sequence is <B, C, D>
- Input sequences **B** batches of subsequences of length **L** randomly sampled from longer sequences of variable length _len_ starting anywhere from index _0_ to _len_-**L**.

The scheduler is Noam Optimizer, discussed in the paper Attention is All You Need.
The Loss function is cross entropy with label smoothing.

## Instructions

`process_midi.py`

`train.py`
