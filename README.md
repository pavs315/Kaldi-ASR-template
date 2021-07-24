# Instructions for making a simple ASR model in Kaldi

## Train and Test Data

### Audio Data

Create Test and Train folders in the Audio folder and store the audio data.

### Acoustic and Language Data

Create Test and Train folders in the Data folder with the following files in each folder.

- spk2gender `<speakerID><gender>'
- wav.scp `<uterranceID> <full_path_to_audio_file>`
- text `<uterranceID> <text_transcription>`
- utt2spk `<uterranceID> <speakerID>`

Create a folder Local in the Data folder with the following files -

- corpus.txt `<text_transcription>`
- lexicon.txt - Can be obtained from http://www.speech.cs.cmu.edu/tools/lextool.html `<word> <phone 1> <phone 2> ...`
- nonsilence_phones.txt `<phone>`
- silence_phones.txt - ``` sil
                           spn
                           ```



