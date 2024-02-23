# AI-Vtuber
This code is designed to read chat messages from YouTube and then utilize OpenAI's GPT-3 language model to generate responses. The output from GPT-3 is then read out loud using a TTS (Text-to-Speech) engine provided by ElevenLabs.



# Setup
Install dependencies
```
git clone https://github.com/Koischizo/AI-Vtuber/
cd AI-Vtuber
pip install -r requirements.txt
```
It also requires [`ffmpeg`](https://ffmpeg.org/) to be installed

# Usage

Edit the variables `EL_key` and `OAI_key` in `config.json`

`EL_key` is the API key for [ElevenLabs](https://beta.elevenlabs.io/). Found in Profile Settings

`OAI_key` is the API key for OpenAI. Found [here](https://platform.openai.com/account/api-keys)

Then run `run.py`

### Default TTS
```
python run.py -id STREAMID 
```
### Elevenlabs TTS
```
python run.py -id STREAMID -tts EL 
```
then you're set
## Notes
Replace `STREAMID` with the stream's ID that you can find on the Youtube Stream link

You can change the voice by changing `voice` in `config.json`. You can find the ID's [here](https://api.elevenlabs.io/docs) in `Get Voices`


