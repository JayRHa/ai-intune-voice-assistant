<!-- unified-readme:start -->
<div align="center">

# AI Intune Voice Assistant

**Archived AI voice assistant experiment for Microsoft Intune administration workflows.**

Build. Automate. Share.

[![GitHub stars](https://img.shields.io/github/stars/JayRHa/AIIntuneVoiceAssistant?style=for-the-badge&logo=github&color=f4c542)](https://github.com/JayRHa/AIIntuneVoiceAssistant/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/JayRHa/AIIntuneVoiceAssistant?style=for-the-badge&logo=github&color=4078c0)](https://github.com/JayRHa/AIIntuneVoiceAssistant/network/members)
[![GitHub issues](https://img.shields.io/github/issues/JayRHa/AIIntuneVoiceAssistant?style=for-the-badge&logo=github&color=d73a4a)](https://github.com/JayRHa/AIIntuneVoiceAssistant/issues)
[![Contributors](https://img.shields.io/github/contributors/JayRHa/AIIntuneVoiceAssistant?style=for-the-badge&logo=github&color=28a745)](https://github.com/JayRHa/AIIntuneVoiceAssistant/graphs/contributors)

---

`Endpoint Management` | `Python` | `Public` | `Maintained`

</div>

## What is this?

This repository provides archived AI voice assistant experiment for Microsoft Intune administration workflows.

> Browse the documentation below for setup notes, usage details, and project-specific context.

---

## Quick Start

1. Review the project documentation below.
2. Clone the repository:

   ```bash
   git clone https://github.com/JayRHa/AIIntuneVoiceAssistant.git
   ```

3. Follow the setup, deployment, or usage notes in the preserved documentation section.

---
<!-- unified-readme:end -->

## Existing Documentation

# Endpoint Analytics Remediation Scripts

## Intro
This script allows users to interact with a voice assistant that is designed to answer questions related to Microsoft Intune. The assistant is friendly, concise, and provides factual answers to queries. It does not provide answers that are not related to Microsoft products or Intune.

## Blog post
https://jannikreinhard.com/2023/04/23/intune-ai-voice-bot/

## Contribution
<table>
  <tbody>
    <tr>
        <td align="center"><a href="https://github.com/Fadope1"><img src="https://avatars.githubusercontent.com/u/68806729?v=4" width="100px;" alt="Fabian Peschke"/><br /><sub><b>Fabian Peschke</b></sub></a><br /><a href="https://www.linkedin.com/in/fabian-peschke-a55554250/" title="LinkedIn">💬</a></td>
        <td align="center"><a href="https://github.com/JayRHa"><img src="https://avatars.githubusercontent.com/u/73911860?v=4" width="100px;" alt="Jannik Reinhard"/><br /><sub><b>Jannik Reinhard</b></sub></a><br /><a href="https://twitter.com/jannik_reinhard" title="Twitter">💬</a> <a href="https://www.linkedin.com/in/jannik-r/" title="LinkedIn">💬</a></td>
  </tbody>
</table>

## Requirements
- Python 3.6 or higher
- Azure Cognitive Services Speech SDK
- OpenAI Python library

You can install the required libraries using pip:
```python
pip install azure-cognitiveservices-speech
pip install openai
```

## Configuration
Before running the script, you must set the following variables with the appropriate values:

- speech_key: Your Azure Cognitive Services Speech subscription key.
- speech_region: The region of your Azure Cognitive Services Speech service (e.g., "eastus").
- language: The language for speech recognition and synthesis (e.g., "en-US").
- voice: The voice for speech synthesis (e.g., "en-US-JennyMultilingualNeural").
- openai.api_key: Your OpenAI API key.
- openai.api_base: The base URL for the OpenAI API (e.g., "https://XXXXXXX.openai.azure.com/").
- deployment_id: The deployment ID for GPT-3.5 Turbo (e.g., "gpt-35-turbo").

You can find more informations here: https://learn.microsoft.com/en-us/azure/cognitive-services/speech-service/language-support?tabs=stt

## Usage
Run the script with the command:
```
python intune_voice_assistant.py
```

The voice assistant will begin listening for input. You can ask questions by starting with "Hey" followed by your query. To reset the conversation context, say "Reset." To stop the conversation, say "Stop" or press Ctrl-Z.
