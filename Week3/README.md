# Week 3: USB Speaker and Audio Output Control with Raspberry Pi

This folder contains the Week 3 Raspberry Pi audio-output notebook.

The experiment shows how to connect a USB speaker to the Raspberry Pi Zero 2 W, detect the device, test audio playback, generate audio tones in Python, visualize waveforms, and use simple Computing with Words / fuzzy-style reasoning to select audio feedback.

## Main Files

- Week3_USB_Speaker_Audio_Output_Control.ipynb  
  Main Jupyter Notebook for the experiment.

- Week3_USB_Speaker_Audio_Output_Control.html  
  Exported HTML version of the executed notebook for quick viewing.

- requirements.txt  
  Python packages required for running the notebook.

## Hardware Used

- Raspberry Pi Zero 2 W
- MicroSD card with Raspberry Pi OS
- USB OTG cable
- USB speaker
- Power supply
- Laptop for SSH/Jupyter access

## Main Experiment Flow

1. Connect the USB speaker to the Raspberry Pi using the USB OTG cable.
2. Check whether the USB speaker is detected using lsusb.
3. Check available playback devices using aplay -l.
4. Test audio output using speaker-test.
5. Generate low, medium, and high tones using Python.
6. Play the generated audio tones through the USB speaker.
7. Visualize the generated audio waveforms.
8. Use simple fuzzy-style reasoning to select audio feedback.
9. Explore a monitoring example using risk, confidence, and urgency.

## Note

In this setup, the USB speaker appears as Jieli Technology UACDemoV1.0.

The playback device is usually plughw:1,0.

Therefore, playback commands in the notebook use:

aplay -D plughw:1,0 filename.wav

If the USB speaker is not detected, reconnect the speaker, check the OTG cable, and run lsusb and aplay -l again.
