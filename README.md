# ModuleTurkishLanguagePack

Complete Turkish language pack for MikoPBX including UI translations and TTS-generated voice prompts.

## What's Included

- **Voice Prompts**: 251 Turkish voice prompts (22050 Hz, mono, 16-bit PCM WAV)
- **UI Translations**: Complete Turkish translation of MikoPBX admin interface
- **Text Mapping**: `Sounds/core-sounds-tr-tr.txt` — full list of prompts with text

## TTS Attribution

Voice prompts were generated using neural TTS (Text-to-Speech) technology:

- **Engine**: [Piper TTS](https://github.com/rhasspy/piper)
- **Voice model**: `tr_TR-dfki-medium`
- **Sample rate**: 22050 Hz
- **Format**: WAV (PCM signed 16-bit, mono)
- **License**: CC BY-SA 4.0

The text for each prompt is stored in `Sounds/core-sounds-tr-tr.txt` for reference and regeneration.

On module installation, MikoPBX automatically converts WAV files to all Asterisk formats (ulaw, alaw, gsm, g722, sln) for optimal codec compatibility.

Tone and silence prompts (e.g. `beep`, `silence/1`, `confbridge-join`) are not synthesized; they are provided as-is from the official Asterisk release.

## Installation

1. Download and install the module from MikoPBX Marketplace
2. Enable the module in **Modules** section
3. Go to **General Settings** and select Turkish (Türkçe) as the system language

## Requirements

- MikoPBX 2025.1.1 or later

## License

- Module code: GNU General Public License v3.0
- Sound files: CC BY-SA 4.0
- TTS engine: Piper TTS (https://github.com/rhasspy/piper)

## Copyright

- Module development: © 2017-2026 Alexey Portnov and Nikolay Beketov
- Voice synthesis: Generated using open-source TTS models
- Remaining system sounds (silence, tones): From official Asterisk release (CC BY-SA 4.0)
