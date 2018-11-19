---
layout: page
title: My Setup
permalink: /setup/

equipment:
  - name: PC
    items:
      - name: CPU
        value: Intel i7-7700 @ 4.20GHz
      - name: GPU
        value: GeForce GTX 1070
      - name: RAM
        value: 32GB
      - name: Primary monitor
        value: Asus 21" @ 1920x1080
      - name: Secondary monitor
        value: Acer 17" @ 1440x900
  - name: Audio
    items:
      - name: Sound card
        value: FocusRite Pro 14
        link: https://reverb.com/uk/p/focusrite-saffire-pro-14?gclid=CjwKCAiAuMTfBRAcEiwAV4SDkefCq-bvAra-k8TZtEPzJeZOcSxqptECxktMT5HBezQ5ka3DSPI2gxoCNNcQAvD_BwE&gclsrc=aw.ds&hfid=8403974
      - name: Analog mixer
        value: Behringer Phenyx 802
        link: https://www.amazon.co.uk/Behringer-802-Input-Bus-Mixer/dp/B000J5XS3C
      - name: Main microphone
        value: Behringer XM8500
        link: https://www.amazon.co.uk/Behringer-XM8500-Ultravoice-Cardioid-Microphone/dp/B0002KZAKS
      - name: Headset microphone
        value: ModMic 5
        link: https://antlionaudio.com/products/modmic-5
      - name: 3.5mm to XLR adapter
        value: Røde VXLR+
        link: https://www.rode.com/accessories/vxlrplus
      - name: Headphones
        value: AKG K52
        link: https://www.amazon.co.uk/AKG-K52-Closed-Back-Headphones/dp/B019EACGSU
      - name: Speakers
        value: Behringer MS-16
        link: https://www.amazon.co.uk/Behringer-MS16-Personal-Monitor-System/dp/B00181T20O
      - name: Audio switch
        value: HQ 3-way switch
        link: https://www.amazon.co.uk/HQ-3-Way-Stereo-Input-Control-black/dp/B000I8OOS8
  - name: Peripherals
    items:
      - name: Webcam
        value: Logitech C920
        link: https://www.logitech.com/en-gb/product/hd-pro-webcam-c920
      - name: Button panel
        value: Stream Deck (15 button)
        link: https://www.elgato.com/en/gaming/stream-deck
      - name: Head tracker
        value: EDTracker Pro
        link: http://edtrackerpro.mybigcommerce.com
  - name: Software
    items:
      - name: OS
        value: Windows 10
      - name: Audio router
        value: VoiceMeeter Banana
        link: https://www.vb-audio.com/Voicemeeter/banana.htm
      - name: VST host
        value: MiniHost Modular
        link: https://www.image-line.com/support/flstudio_online_manual/html/plugins/Minihost%20Modular.htm
      - name: Streaming
        value: StreamLabs OBS
        link: https://streamlabs.com/streamlabs-obs
---
Yes yes, this is _yet another_ streaming setup guide. But the thing about these guides is that you can cherry pick from other people's setups and figure out a system that _really_ works for you. So here's mine, have at it.

**Note: this is currently an unfinished work in progress**

## Overview

I run a single PC setup with two monitors and two soundcards, configured in such a way that I can use my system for more than just streaming, and can use my hardware for listening to music, watching movies, and for plugging in instruments and other external audio devices.

## Requirements

When designing my setup, I wanted:

* My primary monitor dedicated to games, and a secondary monitor to observe stream status, chat, etc.
* A headset microphone when head tracking so my voice level doesn't change as I look around, and a better quality static microphone for everything else.
* To be able to independently manage audio channels such as microphone, voice chat, music and desktop sounds.
* To be able to use my speakers without feedback from my microphone.
* To be able to plug in musical instruments and other external audio devices and play them through my speakers.
* To be able to control as much as possible without having to click around between applications.

## Equipment

<table>
  <tbody>
    {% for group in page.equipment %}
    <tr><th colspan="2" style="background:#9e9e9e;color:#fff;"><strong>{{group.name}}</strong></th></tr>
    {% for item in group.items %}
    <tr>
      <th width="30%">{{item.name}}</th>
      <td>
        {% if item.link %}
        <a href="{{item.link}}" target="_blank">{{item.value}}</a>
        {% else %}
        {{item.value}}
        {% endif %}
      </td>
    </tr>
    {% endfor %}
    {% endfor %}
  </tbody>
</table>
