# talking-tree-pi
The aim of this project is to develop a conversational tree to raise awareness of environmental stressors :deciduous_tree:. To achieve this, we are focusing on developing an LLM that runs on a Raspberry Pi 5.

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

Install additional packages: <br>
- install requests package for sending HTTP requests `sudo apt install python3-requests`
- install scipy package for scientific computing and technical computing `sudo apt install python3-scipy`
- install numpy package for multi-dimensional arrays `sudo apt install python3-numpy`

### install whisper on a raspberry pi

install faster-whisper on a rapsberry pi: <br>
`sudo apt update`<br>
`sudo apt install python3-pip python3-venv` <br>

Create a virtual environment: <br>
`spython3 -m venv whisper-envs` <br>

Activate it: <br>
`source whisper-env/bin/activate`<br>

Now install faster-whisper:<br>
`pip install faster-whisper`<br>

Then, install sounddevice: <br>
`pip install sounddevice`<br>

Install piper-tts package for local text-to-speech: <br>
`pip install piper-tts`<br>
and <br>
Install onnxruntime for ONNX models <br>
`pip install onnxruntime` <br>



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








