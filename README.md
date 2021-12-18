# Project: Audio Documentation

Project Audio is a project for DiamondFire plots that allow you to play full quality audio through our api!

Here you can find documentation for v2 of our API!

## API Docs
[Playing Audio](#Playing%20Audio)

[Stopping Audio](#Stopping%20Audio)

[Audio Sources](#Audio%20Sources)


## Playing Audio

Playing audio with **Project Audio** is easy you send a URL **post request** from your plot using DiamondFire's **[SendWebRequest](#SendWebRequest%20CodeBlock)** code block!

The URL format is as follows https://audio.tomoli.me/api/v2/play/[player](#Player%20Paramater)/[title](#Title%20Paramater)/[loop](#Loop%20Paramater)/

The [audio source](#Audio Sources) should be placed in the body.

## Stopping Audio

Stopping audio with **Project Audio** is easy you send a URL **post request** from your plot using DiamondFire's **[SendWebRequest](#SendWebRequest%20CodeBlock)** code block!

The URL format is as follows https://audio.tomoli.me/api/v2/stop/[player](#Player%20Paramater)/

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

## Paramaters

Paramaters are sections of the URL that you substitute in for your data!

### Player Paramater

This is the player’s username you want to play the music to. The player must be on your plot.
*You may also use multiple players by joining there names with a , for example: TechStreet,Tomoli75)*

### Title Paramater

This is the title that will show up in the web interface. Preferably, this will be the song title or the announcement title - e.g. if you wish to rick-roll people listening, you would put “Never Gonna Give You Up - Rick Astley” as the title.

**You must encode this with URL encoding documentation for this can be found [here](https://www.w3schools.com/tags/ref_urlencode.ASP)**

### Loop Paramater

This should be either true or false. If true, the audio will loop.

## SendWebRequest CodeBlock
![SendWebRequest](https://raw.githubusercontent.com/DF-Project-Audio/Documentation/main/images/SendWebRequest.png)
