<img align="right" src="https://i.imgur.com/zrE80HY.png" height="200" width="200">

# JMusicBot

[![Release](https://img.shields.io/github/release/msbeaule/MusicBot.svg)](https://github.com/msbeaule/MusicBot/releases/latest)
[![License](https://img.shields.io/github/license/msbeaule/MusicBot.svg)](https://github.com/msbeaule/MusicBot/blob/master/LICENSE)

A fork of a cross-platform Discord music bot with a clean interface, and that is easy to set up and run yourself!

[![Setup](http://i.imgur.com/VvXYp5j.png)](https://jmusicbot.com/setup)

## Features

  * Easy to run (just make sure Java is installed, and run!)
  * Fast loading of songs
  * No external keys needed (besides a Discord Bot token)
  * Smooth playback
  * Server-specific setup for the "DJ" role that can moderate the music
  * Clean and beautiful menus
  * Supports many sites, including YouTube, SoundCloud, and more
  * Supports many online radio/streams
  * Supports local files
  * Playlist support (both web/YouTube, and local)

## Supported sources and formats

JMusicBot supports all sources and formats supported by [LavaPlayer](https://github.com/lavalink-devs/lavaplayer#supported-formats):

### Sources

  * YouTube
  * SoundCloud
  * Bandcamp
  * Vimeo
  * Twitch streams
  * Local files
  * HTTP URLs

### Formats

  * MP3
  * FLAC
  * WAV
  * Matroska/WebM (AAC, Opus or Vorbis codecs)
  * MP4/M4A (AAC codec)
  * OGG streams (Opus, Vorbis and FLAC codecs)
  * AAC streams
  * Stream playlists (M3U and PLS)

## Example

![Loading Example...](https://i.imgur.com/kVtTKvS.gif)

## Setup

Please see the [Setup Page](https://jmusicbot.com/setup) to run this bot yourself!

## Questions/Suggestions/Bug Reports

**Please read the [Issues List](https://github.com/jagrosh/MusicBot/issues) before suggesting a feature**. If you have a question, need troubleshooting help, or want to brainstorm a new feature, please start a [Discussion](https://github.com/jagrosh/MusicBot/discussions). If you'd like to suggest a feature or report a reproducible bug, please open an [Issue](https://github.com/jagrosh/MusicBot/issues) on this repository. If you like this bot, be sure to add a star to the libraries that make this possible: [**JDA**](https://github.com/DV8FromTheWorld/JDA) and [**LavaPlayer**](https://github.com/lavalink-devs/lavaplayer)! 

## Editing

This bot (and the source code here) might not be easy to edit for inexperienced programmers. The main purpose of having the source public is to show the capabilities of the libraries, to allow others to understand how the bot works, and to allow those knowledgeable about java, JDA, and Discord bot development to contribute. There are many requirements and dependencies required to edit and compile it, and there will not be support provided for people looking to make changes on their own. Instead, consider making a feature request (see the above section). If you choose to make edits, please do so in accordance with the Apache 2.0 License.

### Compiling / Building Tips

First [download java JDK and JRE](https://www.openlogic.com/openjdk-downloads), and add both to your PATH environment variable.

[Download](https://maven.apache.org/download.cgi) and [install Maven](https://maven.apache.org/install.html). Then inside the Maven folder, find `mvn.cmd` and add your JDK version to it (unless you already have the JAVA_HOME environment variable set already). This is the path to the base folder, don't include /bin:

```bat
set JAVA_HOME=<path/to/JDK/folder>
```

In a terminal/cmd window in the directory of the music bot (same folder as the `pom.xml` file), run `mvn package` to create the .jar file in the `target/` folder.

Inside the `target/` folder, you can then run `JMusicBot-Snapshot-All.jar` with the java JRE version that matches the one you created it with. Hopefully if it all went well, the bot will run.
