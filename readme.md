## Description

OpenVoiceOS plugin for Microsoft Azure

## Install

```bash
pip install ovos-stt-plugin-azure
```

## Configuration

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

`key` - key for Azure AI services API

`region`: location/region for your Azure speech service

`profanity`: profanity filter setting, possible values are `raw`, `masked`, or `removed`
