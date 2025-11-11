**ESPHome ESP32-S3 Box 3**

This project is based on the official ESPHome Wake Word Voice Assistant example: https://github.com/esphome/wake-word-voice-assistants/blob/main/esp32-s3-box-3/esp32-s3-box-3.yaml

**Overview**

The goal of this configuration is to extend the ESP32-S3 Box 3 into a smart home control station — not just a voice assistant.

**It includes:**

A custom home (idle) page with four icons, visually designed by Sora.

Additional control and automation functions layered on top of the voice assistant features.

**Gotchas:**
For the lights, if yours is controlled by a smart switch, in home assistant > setting > device > helper, you can create a new helper to convet from switch to light. Otherwise, light.toggle won't work on it.


**Voice Assistant**

As the core function of this device, I uses OpenAI as the conversational agent.
While responses may have a 3–5 second delay, the understanding of natural English — especially for non-native speakers — is significantly better.

**Limitation/To improve**
Volume control/Brightness control is one way (touch screen -> Media player/esp32), trying to figure out the Esphome API two way sync.

**Credits**

Special thanks to BigBobbas for sharing his fonts and ideas, which inspired and improved this project.
