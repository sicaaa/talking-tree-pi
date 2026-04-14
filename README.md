# talking-tree-pi
The aim of this project is to develop a conversational tree to raise awareness of environmental stressors :deciduous_tree:. To achieve this, we are focusing on developing an LLM that runs locally on a Raspberry Pi 5.

## getting started with raspberry pi
To get started, go to the raspberry documentation website: </br>
https://www.raspberrypi.com/documentation/computers/getting-started.html </br>

Then, download the Raspberry Pi OS (64-bit) Full.</br>
https://www.raspberrypi.com/software/operating-systems/ </br>

Install Raspberry Pi OS on a SD card by using the Raspberry Pi Imager : </br>
https://www.raspberrypi.com/software/</br>


## install

### install VS code 
Install an editor on your Raspberry Pi: <br>
https://code.visualstudio.com/docs/setup/raspberry-pi <br>

You can install it by running: <br>
`sudo apt update` <br>
`sudo apt install code`

Update VS Code: <br>
`sudo apt update` <br>
`sudo apt upgrade code`

### install python
Install Python on your Raspberry Pi: <br>
https://www.python.org <br>

- open the terminal and make sure you are using the correct Python installation: `python3 --version`
- upgrade pip `python3 -m pip install --upgrade pip`

Then, install additional packages via the terminal by using pip or pip3: <br>

- install faster-whisper package for fast speech-to-text `pip3 install faster-whisper`
- install requests package for sending HTTP requests `pip3 install requests`
- install sounddevice package for audio input/output `pip3 install sounddevice`
- install scipy package for scientific computing and technical computing `pip3 install scipy`
- install numpy package for multi-dimensional arrays `pip3 install numpy`
- install piper-tts package for local text-to-speech `pip3 install piper-tts`
- install onnxruntime for ONNX models `pip3 install onnxruntime`


### install ollama
With Ollama, you can run large AI language models locally on your computer. </br>
To get started, download Ollama on macOS: </br>
https://ollama.com/download

Then, download a small ai model, such as tinyllama or gemma:2b: </br>
https://ollama.com/library/tinyllama


### install piper
Piper is a fast and local neural text-to-speech engine. <br>
To get started, go to the following repository and install piper: <br>
https://github.com/OHF-Voice/piper1-gpl <br>
For installing piper you can find unseful istructions here: <br>
https://www.thoughtasylum.com/2025/08/25/text-to-speech-on-macos-with-piper/ <br>

- open the terminal and install piper: `pip3 install piper-tts`

If the installation via pip fails you can download the following file for your macOS: <br>
https://sourceforge.net/projects/piper-tts.mirror/files/2023.11.14-2/piper_macos_aarch64.tar.gz/download <br>


### piper voices
Test different piper voices here: <br>
https://piper.ttstool.com/ <br>

Then, download the following piper voice model here: <br>
https://huggingface.co/rhasspy/piper-voices/tree/main/de/de_DE <br>

In this proof of concept we used thorstens voice: <br>
- de_DE-thorsten-high.onnx
- de_DE-thorsten-high.onnx.json








