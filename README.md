# AudioDataset

A list of audio datasets that I often used

## Speech
* [VCTK v0.92](https://datashare.ed.ac.uk/handle/10283/3443). 110 English speakers with various accents, each of them reads out about 400 sentences. All recordings were converted 48 kHz,
  - trainset size **TBD**
* [VoiceBanK-DEMAND](https://datashare.ed.ac.uk/handle/10283/2791)
  - Single channel human speech, 48 kHz.
  - Noisy speech are corrupted by noise from [DEMAND datasets](https://zenodo.org/records/1227121)
  - 28 speakers version, trainset has 11572 utterances (~ 9.4 hours), testset has 824 utterances (~ 0.6 hours). Usually, following [MetricGanU](https://arxiv.org/abs/2110.05866), we downsample to 16kHz and split p226 & p287 from the trainset for validation, which consists of 770 utterances (~ 0.6 hours), the rest trainset consists of 10802 utterance (~ 8.8 hours).
  - 56 speakers version, **TBD**
* [LibriSpeech](https://www.openslr.org/12), ~ 1000 hours of 16kHz read English speech corpus, **TBD**
  - trainset: 100 hours + 360 hours + 500 hours (960 hours in total, )
  - dev-clean/other:
  - test-clean/other:
* [Libri-light](https://github.com/facebookresearch/libri-light/blob/main/data_preparation/README.md), contain unlabled speech corpus around 60k hours
  - small: 577 hours
  - medium: 5,193 hours
  - large: 51,934 hours
* [DNS-Challenge 5](https://github.com/microsoft/DNS-Challenge), contain multilingual clean speech and various noise in 
  - Clean Speech: 
  - Noise


  
## Music
* [StarNet](https://zenodo.org/records/6917099). Classical music pieces obtained from their corresponding free MIDI files,
  - 104 tracks in 48 kHz.
  - Tracks:
    - xxx.0.wav: the clarinet-vibraphone mixture
    - xxx.1.wav: the clarinet track
    - xxx.2.wav: the vibraphone track
    - xxx.3.wav: the strings-piano mixture
    - xxx.4.wav: the strings track
    - xxx.5.wav: the piano track 


## Audio Mixture
* [Libri2Mix](https://github.com/JorisCos/LibriMix), **TBD**
* [AudioSet](https://research.google.com/audioset/index.html), general audio corpus
  - unbalanced audio:
  - balanced audio: 
* [Divide and Remaster (DnR)](https://zenodo.org/records/6949108)
  - Single channel mixture with speech, music, and sound effects/background stems, 44.1 kHz
  - Audio source: librispeech (speech), free music archive (music), FSD50k (sound effect)
  - Cinematic demixing challenge ([link](https://www.aicrowd.com/challenges/sound-demixing-challenge-2023/problems/cinematic-sound-demixing-track-cdx-23))
  - Each utterance is 60s, with 3,406 mixtures (∼ 57 h) for the training set, 487 mixtures (∼ 8 h) for the validation set, and 973 mixtures ( ∼16 h) for the test set
* [MUSAN](https://www.openslr.org/17/)
  - A corpus of music, speech and noise in 16 kHz, suitable for voice activity detection (VAD) and music/speech discrimination
  - Speech: 426 utterances (~ 60 hours), source from LibriVox and US Gov
  - Music: 660 utterances (~ 42 hours), source from Jamendo, Free Music Archive, Incompetech, and HD Classical Music
  - Noise: 930 utterances (~ 6 hours), source from Free Sound and Sound Bible
