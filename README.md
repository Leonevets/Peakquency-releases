<p align="center">
  <img src="docs/readme/hero.png" alt="Peakquency. A voice-activated soundboard." width="880">
</p>

<p align="center">
  <strong>Say it, press it, or click it.</strong><br>
  The people in your Discord call, game, or meeting hear the sound too. You hear it in your headphones at the same time.
</p>

<p align="center">
  <a href="https://github.com/Leonevets/Peakquency-releases/releases/download/v0.60.2/Peakquency-Setup-0.60.2.exe"><img alt="Download Peakquency Setup 0.60.2" src="https://img.shields.io/badge/Setup-0.60.2-8B5CF6?style=for-the-badge&logo=windows&logoColor=white"></a>
  &nbsp;
  <a href="https://github.com/Leonevets/Peakquency-releases/releases/download/v0.60.2/Peakquency-0.60.2-win-x64-portable.zip"><img alt="Download the portable zip 0.60.2" src="https://img.shields.io/badge/Portable_zip-0.60.2-312E81?style=for-the-badge"></a>
  &nbsp;
  <a href="https://github.com/Leonevets/Peakquency-releases/releases"><img alt="All Peakquency releases" src="https://img.shields.io/badge/All_releases-GitHub-1e1b4b?style=for-the-badge&logo=github&logoColor=white"></a>
</p>

<p align="center">
  Windows 10 or 11 &nbsp;·&nbsp; English, Spanish, French, German, Japanese &nbsp;·&nbsp; Speech stays on your PC
</p>

<p align="center">
  <img src="docs/readme/wave.png" alt="A purple waveform with a mountain peak in the middle." width="520">
</p>

## The board

<p align="center">
  <img src="docs/readme/board.png" alt="The Peakquency board. Voice and Hotkeys are on. Airhorn, Vine boom, Correct, and Bell each have a phrase, a hotkey, and a volume." width="880">
</p>

Play sends a sound to you and to the call. Preview is only for you. Say the phrase, hit the hotkey, or press play. Categories, search, and sort keep a big board easy to scan. A blocking phrase, like not correct on Correct, keeps that one sound quiet.

## Say a phrase

<p align="center">
  <img src="docs/readme/phrases.png" alt="The phrase guide. airhorn matches air horn. airhorn! still plays. The longer phrase wins." width="520">
</p>

The guide sits beside the board, so you can try a phrase while you read it. Spaces inside a phrase do not matter. Punctuation is ignored. The longer phrase wins, and only the stop phrase by itself stops everything.

## Shape the clip

<p align="center">
  <img src="docs/readme/editor.png" alt="The clip editor open on Vine boom, with the waveform, trim handles, fade, and save buttons." width="880">
</p>

Trim the start and the end, cut a piece out of the middle, and set a fade. Play in here is a preview, and only you hear it. Save as a new sound, or overwrite this one.

## Also in there

- **Two ways out.** Play the sounds on the real microphone, or into a virtual cable such as VB-Cable. Then set Discord, your game, or your call to that input. Turn Discord's noise suppression off, or it throws away sounds that are not a voice.
- **Listening.** Always, hold to listen, hold to pause, toggle, or leave the microphone out. The call still hears you the same. A stop key and a stop phrase end everything that is playing.
- **Speech stays here.** Whisper runs on this PC, on the graphics card or the processor. Nothing you say is sent anywhere. Bigger models hear more clearly. Tiny is lighter while a game is running.
- **While a sound plays.** Other phrases can wait. A stop phrase still gets through. Hotkeys and the play button never wait on a cooldown.
- **Your window.** Cozy is the darker purple look, or follow Windows. Compact fits more sounds on screen. Close can leave Peakquency running by the clock. It can start with Windows, in the window or hidden.
- **Boards you can carry.** A preset is the whole board, sounds included. Save a board to a file and load it on another Peakquency, with the audio or with just the layout.
- **Files.** Sounds, presets, settings, and speech models live next to the program when that folder is writable, and in `%LOCALAPPDATA%\Peakquency` when it is installed. Drop in WAV, MP3, FLAC, M4A, AAC, WMA, AIFF, Ogg Vorbis, Opus, AC-3, or DTS. A video comes in as its audio.

`Peakquency-Setup-0.60.2.exe` installs to Program Files and adds the .NET 8 Desktop Runtime when it is missing. The first question is the language. `Peakquency-0.60.2-win-x64-portable.zip` is a folder you can copy and run, runtime included.

Removing the program puts every microphone that was activated for sounds back the way it was. If one was activated, uninstall warns that audio drops out for a moment. It can also delete the Peakquency folders. A sounds folder you moved in Settings is left alone.

From a copy of the source:

```powershell
dotnet build Peakquency.sln
dotnet run --project src\Peakquency
dotnet test Peakquency.sln
installer\package.ps1
```
