# 21Codec

Streaming neural speech codec with decoder-side speaker control.

21Codec encodes speech at 0.80 kbps (50 Hz, 16 bits per frame) with reduced
recoverable speaker identity in the token stream, and supplies identity at the
decoder as a single speaker embedding that conditions every frame. Identity is
therefore fixed across chunk boundaries during streaming decoding, and can be
changed mid-stream at no additional bitrate.

This repository accompanies a paper submitted to ICASSP 2026.

## Status

Code release is planned upon acceptance.

**Planned for release**

- Training pipeline: codec, discriminators, and the adversarial speaker probe
- Inference pipeline, including chunk-causal streaming decoding

**Not planned for release**

- Pretrained checkpoints. Part of the training mixture is in-house data we
  cannot redistribute, so we are not able to release weights derived from it.

## Citation

To be added upon acceptance.
