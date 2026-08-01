## Description

OVOS STT plugin for [Microsoft Azure AI Speech](https://azure.microsoft.com/en-us/products/ai-services/ai-speech). It sends audio to the Azure speech-to-text REST API and returns the recognized text.

This plugin is part of the [OpenVoiceOS](https://github.com/OpenVoiceOS) speech-to-text (STT) plugin family. See the [OVOS Plugin Manager](https://github.com/OpenVoiceOS/OVOS-plugin-manager) for the STT plugin interface these plugins implement.

## Install

```bash
pip install ovos-stt-plugin-azure
```

## Configuration

Add this plugin to the `stt` section of your OVOS configuration.

```json
  "stt": {
    "module": "ovos-stt-plugin-azure",
    "ovos-stt-plugin-azure": {
      "key": "xxx",
      "region": "westeurope",
      "profanity": "raw"
    }
  }
```

- `key`: key for the Azure AI Speech API.
- `region`: location or region of your Azure speech service.
- `profanity`: profanity filter setting. Valid values are `raw`, `masked`, or `removed`.

## License

This project uses the [Apache 2.0 License](LICENSE).
