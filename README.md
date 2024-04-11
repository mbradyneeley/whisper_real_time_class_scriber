# Real Time Whisper Transcription

![Demo gif](demo.gif)

This is straightforward code of real time speech to text with OpenAI's Whisper model. It works by constantly recording audio in a thread and concatenating the raw bytes over multiple recordings.

I have implemented 8bit quantization of the whisper model to speed things up. In most cases this actually improves the model's
performance (https://github.com/MiscellaneousStuff/openai-whisper-cpu)

To install dependencies simply run
```
pip install -r requirements.txt
```
in an environment of your choosing.

Whisper also requires the command-line tool [`ffmpeg`](https://ffmpeg.org/) to be installed on your system, which is available from most package managers:

```
# on Ubuntu or Debian
sudo apt update && sudo apt install ffmpeg

# on Arch Linux
sudo pacman -S ffmpeg

# on MacOS using Homebrew (https://brew.sh/)
brew install ffmpeg

# on Windows using Chocolatey (https://chocolatey.org/)
choco install ffmpeg

# on Windows using Scoop (https://scoop.sh/)
scoop install ffmpeg
```

For more information on Whisper please see https://github.com/openai/whisper

The code in this repository is public domain.

Originally forked from:
https://github.com/davabase/whisper_real_time
