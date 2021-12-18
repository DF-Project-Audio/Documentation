# Project: Audio Documentation

Project Audio is a project for DiamondFire plots that allow you to play full quality audio through our api!


## Playing Audio

Playing audio with **Project Audio** is easy you send a URL **post request** from your plot using DiamondFire's **SendWebRequest** code block!
![SendWebRequest](https://raw.githubusercontent.com/DF-Project-Audio/Documentation/main/images/SendWebRequest.png)

The URL format is as follows https://audio.tomoli.me/api/v2/play/[player](#Player Paramater)/[title](#Title Paramater)/[loop](#Loop Paramater)/

The [audio source](#Audio Sources) should be placed in the body.

## Stopping Audio

Stopping audio with **Project Audio** is easy you send a URL **post request** from your plot using DiamondFire's **SendWebRequest** code block!
![SendWebRequest](https://raw.githubusercontent.com/DF-Project-Audio/Documentation/main/images/SendWebRequest.png)

The URL format is as follows https://audio.tomoli.me/api/v2/stop/[player](#Player Paramater)/

## Audio Sources

There are many ways to directly provide audio to play in Project Audio!

### Direct URL
This should be provided by you, and is perfect for maximum customisation. Just provide the web-accessable url, ending with a file extention like .mp3, as part of the request.

### TTS
We provide free access to the basic (Google Translate style) TTS service from Google. 

The URL format is as follows:
https://audio.tomoli.me/api/v2/source/tts/[text].mp3 *(Replace [text] with the [URL-encoded](https://www.w3schools.com/tags/ref_urlencode.ASP) text you want to use.)*

### GLaDOS TTS
We also provide access to GLaDOS TTS, recommended for use in puzzle-style games. 

The URL format is as follows:
https://audio.tomoli.me/api/v2/source/glados/[text].mp3 *(Replace [text] with the [URL-encoded](https://www.w3schools.com/tags/ref_urlencode.ASP) text you want to use.)*

### YouTube
Furthermore, we provide the ability to play YouTube videos (audio only) via the service. 

The URL format is as follows:
https://audio.tomoli.me/api/v2/source/yt/[id].mp3 *(Replace [id] with the YouTube video id you want to play. For example, dQw4w9WgXcQ plays a rick-roll)*
