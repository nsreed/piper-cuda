# Piper TTS

This project does TTS.

While you can run live cloning on Windows using xtts2, it's a bit slow.

Train a model using xtts2 and deepspeed in this container, to be used anywhere!

See https://docs.coqui.ai/en/latest/models/xtts.html#manual-inference

## Installation

1. Set up Conda
2. Install Requirements
3. Run `verify.py`

## Training

Inputs:
- .wav samples

Outputs:
- tensor checkpoint

## Notes

For deepspeed to work, you may need the libaio-dev apt package
```bash
sudo apt update
sudo apt install libaio-dev
```

Git needs username and email

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@yourdomain.com"
```