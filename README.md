# AudioDataset

A list of audio datasets that I often used

## Speech Enhancement/Separation/Dereverberation

* [VoiceBanK-DEMAND](https://datashare.ed.ac.uk/handle/10283/2791)
  - Single channel human speech, 48 kHz.
  - Noisy speech are corrupted by noise from [DEMAND datasets](https://zenodo.org/records/1227121)
  - 28 speakers version, trainset has 11572 utterances (~ 9.4 hours), testset has 824 utterances (~ 0.6 hours). Usually, following [MetricGanU](https://arxiv.org/abs/2110.05866), we downsample to 16kHz and split p226 & p287 from the trainset for validation, which consists of 770 utterances (~ 0.6 hours), the rest trainset consists of 10802 utterance (~ 8.8 hours).
  - 56 speakers version, **TBD**
* [Libri2Mix](https://github.com/JorisCos/LibriMix), **TBD**
* [Divide and Remaster (DnR)](https://zenodo.org/records/6949108)
  - Single channel mixture with speech, music, and sound effects/background stems, 44.1 kHz
  - Audio source: librispeech (speech), free music archive (music), FSD50k (sound effect)
  - Cinematic demixing challenge ([link](https://www.aicrowd.com/challenges/sound-demixing-challenge-2023/problems/cinematic-sound-demixing-track-cdx-23))
  - Each utterance is 60s, with 3,406 mixtures (∼ 57 h) for the training set, 487 mixtures (∼ 8 h) for the validation set, and 973 mixtures ( ∼16 h) for the test set

## Speech Resynthesis/SSL/TTS

* [VCTK v0.92](https://datashare.ed.ac.uk/handle/10283/3443). 110 English speakers with various accents, each of them reads out about 400 sentences. All recordings were converted 48 kHz,
  - trainset size **TBD**
* [LibriSpeech](https://www.openslr.org/12), ~ 1000 hours of 16kHz read English speech corpus, **TBD**
  - trainset: 100 hours + 360 hours + 500 hours (960 hours in total, )
  - dev-clean:
  - dev-other:
  - test-clean:
  - test-other: 
