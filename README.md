# pydl-audio-encoders
Audio encoders that convert audios into numpy arrays for machine learning

The implementation of the audio is in the [pydl_audio_encoders/library](pydl_audio_encoders/library)

# Usage

### Audio Classifier

The [sample codes](demo/audio_classifier.py) shows how to use the encoder to predict the genre
of a song

### Audio Encoder




# Note

### audioread.NoBackend

The audio processing depends on librosa version 0.6 which depends on audioread.  

If you are on Windows and sees the error "audioread.NoBackend", go to [ffmpeg](https://ffmpeg.zeranoe.com/builds/)
and download the shared linking build, unzip to a local directory and then add the bin folder of the 
ffmpeg to the Windows $PATH environment variable. Restart your cmd or powershell, Python should now be
able to locate the backend for audioread in librosa
