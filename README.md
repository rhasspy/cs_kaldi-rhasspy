# Czech Kaldi Profile

A [Rhasspy](https://github.com/rhasspy/rhasspy) profile for Czech (`cs`).

Includes:

* A [Kaldi nnet3](https://kaldi-asr.org/doc/dnn3.html) speech to text model
    * See files in `acoustic_model/`
    * Recipe created with [ipa2kaldi](https://github.com/rhasspy/ipa2kaldi)
    * Word error rate: 11.03%
    * Trained on:
        * [Vystadial VOIP](http://www.openslr.org/6/) (18.2 hours)
        * [Common Voice](https://commonvoice.mozilla.org) (26.6 hours)
* An [IPA](https://en.wikipedia.org/wiki/International_Phonetic_Alphabet) pronunciation lexicon pulled from [Wiktionary](https://www.wiktionary.org/)
    * See `base_dictionary.txt.gz`
* A [phonetisaurus](https://github.com/AdolfVonKleist/Phonetisaurus) grapheme to phoneme model for predicting word pronunciations
    * See `g2p.fst.gz`
    * Trained on `base_dictionary.txt.gz`
* A tri-gram [ARPA language model](https://cmusphinx.github.io/wiki/arpaformat/)
    * See `base_language_model.txt.gz`
    * Text from audio transcriptions and [Universal Dependencies](https://universaldependencies.org/)
