Teensy 2.0, LC, 3.x, 4.x core libraries for Arduino.

Teensy 4.x modified to parameterise the Audio config, specifically:

- Added audioparams.h
    - allows for 44.1k, 48k, 96k sample rates
    - Affects:
        - AudioStream.h - SAMPLE_RATE_EXACT
        - usb_desc.h - AUDIO_TX_SIZE / AUDIO_RX_SIZE
        - usb_audio.cpp - feedback_accumulator (via usb_audio.h), target (in function - usb_audio_transmit_callback, via usb_audio.h)
        - usb.c - AUDIO_INTERFACE endpoint0_buffer (via usb_audio.h)




The latest stable version of Teensy's core library is always available in the Teensyduino installer, at this page:

http://www.pjrc.com/teensy/td_download.html
