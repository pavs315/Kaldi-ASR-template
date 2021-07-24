# Instructions for making a simple Kaldi recipe

## Train and Test Data

### Audio Data

Create Test and Train folders in the Audio folder and store the audio data.

### Acoustic Data

Create Test and Train folders in the Data folder with the following files in each folder.

- spk2gender `<speakerID><gender>
- wav.scp `<uterranceID> <full_path_to_audio_file>`
- text `<uterranceID> <text_transcription>`
- utt2spk `<uterranceID> <speakerID>`


