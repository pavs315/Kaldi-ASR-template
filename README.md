# Instructions for making a simple HMM-GMM ASR model in Kaldi

## Train and Test Data

### Audio Data

Create Test and Train folders in the Audio folder and store the audio data.

### Acoustic and Language Data

Create Test and Train folders in the Data folder with the following files in each folder.

- spk2gender `<speakerID><gender>`
- wav.scp `<uterranceID> <full_path_to_audio_file>`
- text `<uterranceID> <text_transcription>`
- utt2spk `<uterranceID> <speakerID>`

Create a folder local with the following file and a subfolder dict -

- corpus.txt `<text_transcription>`

Create the follwing files in dict

- lexicon.txt - Can be obtained from http://www.speech.cs.cmu.edu/tools/lextool.html `<word> <phone 1> <phone 2> ...`
- nonsilence_phones.txt `<phone>`
- silence_phones.txt - 

 ```  
  sil
  spn
 ```
- optional_silence.txt

 ```
 sil
 ```

## Utils and Config

Copy the utils and steps folders from `Kaldi-Master/egs/wsj/s5` into the model directory

## Scoring script

Copy `score.sh` from `Kaldi-Master/egs/voxforge/s5/local` into the local folder of the model directory.

## Config files

Create a folder conf in the model directory and copy the decode.config and mfcc.conf files from this repository.

## Running the Model

Copy the files `cmd.sh`, `path.sh` and `run.sh` to the project directory

Run `./run.sh`













