# Char-RNN-TensorFlow - IN PROGRESS

Character generator using recurrent neural network (_RNN_).
Also _Node.js_ server used to provide _HTTP_ API for training 
_RNN_ and then generating samples from saved checkpoints.

## Generator

_Forked_ from [hzy46/Char-RNN-TensorFlow](https://github.com/hzy46/Char-RNN-TensorFlow) 
and is in separate directory (`generator/`) now to avoid confusion. It has its own documentation
in [`generator/README.md`](generator/README.md).

## Server

Trivial _Node.js_ server used to store incoming training data and call `python` scripts to train 
and generate text. Read about it in [`server/README.md`](server/README.md)

## Development

Both `server` and `generator` are wrapped with Docker.

### Build and run

- To `build` container image: `docker build -t <some_name> .`
- To `run` built image: `docker run -p 8080:8080 -ti --rm <some_name>`

## Your feedback

You are free to open issues if there is anything bothering you, I'll read through and will make 
best effort to fix/reply ASAP.
