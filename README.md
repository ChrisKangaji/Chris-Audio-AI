# AI Voice Clone

This project is a real-time voice-based AI assistant that uses:
- **Deepgram** for speech-to-text
- **GPT-4 (OpenAI)** for generating smart replies
- **ElevenLabs** to speak back using your cloned voice

## Features
- Real-time microphone input
- Conversational responses powered by GPT-4
- Outputs voice responses in your own cloned voice

## Required Packages
- **openai** Official OpenAI SDK
- **requests** Standard HTTP library
- **python-dotenv** For loading .env config files
- **deepgram-sdk** Deepgram's official Python SDK
- **websocket-client** Required by Deepgram for real-time audio
- **sounddevice** Lets you record from your microphone and play audio to your speakers in real-time
- **numpy** Convert audio chunks (bytes) into playable waveforms and stream live audio as it’s generated

## Setup
1. Clone the repo
3. Create a .env file (.env.apiKeys) for hold all your api keys na dinclude the following:
    OPENAI_API_KEY=your_openai_api_key
    DEEPGRAM_API_KEY=your_deepgram_api_key
    ELEVENLABS_API_KEY=your_elevenlabs_api_key
    ELEVENLABS_VOICE_ID=your_cloned_voice_id
2. Install dependencies:
```bash
pip install -r requirements.txt
