---
layout: page
title: "Captions and Transcripts for AV material"
permalink: /digitization/captions/
parent: "Digitization: Audiovisual Carriers"
grand_parent: Digitization
nav_order: 2
---
# Captions and Transcripts for Audiovisual Material
Captions and transcripts for audiovisual material make collections material more accessible and enhance the over-all level of access. [^1] Captions should be created in the WebVTT format. Captions can be embedded or burned into access files, but they should not be embedded into master files.

# Tools for Creating and Reviewing Captions

## WhisperAI - Jupyter Notebook Python Script

The Digital Services unit uses [WhisperAI](https://github.com/openai/whisper) via a python script run in a Jupyter Notebook environment to generate WebVTT caption files. This script sets WebVTT metadata values as described in the [Guidelines for Embedding Metadata in WebVTT Files (FADGI)](https://www.digitizationguidelines.gov/guidelines/accessibilty_WebVTT.html)

The WebVTT files generated through this script can be edited in SubtitleEdit. 

## SubtitleEdit 
SubtitleEdit is an open source tool for creating and editing subtitles and captions. SubtitleEdit can also be used as a GUI for WhisperAI.

## Adobe Premiere
The SCRC digitization lab provides access to Adobe Premiere. You may also request a license for your individual workstation via GWU IT.

-[Guide: Creating Captions using Adobe Premiere](https://docs.google.com/document/d/1ZRbPUFNSYGfbZA5lTdnkvejmCeflvuGvMg0Ot4aBwyU/edit?usp=sharing)


# File Naming for Caption and Subtitle Files
WebVTT files should inherent the file name of the AV source file. The file name should also include information about the language to improve accessibility. 

Example:
- *Source AV File*: ms0000_s01_ss02_c03_i01.mp4
- *Language*: eng
- **WebVTT file**: ms0000_s01_ss02_c03_i01_eng.vtt

# Metadata for WebVTT 
See [Guidelines for Embedding Metadata in WebVTT Files (FADGI)](https://www.digitizationguidelines.gov/guidelines/accessibilty_WebVTT.html). Required elements should be used when possible. The following elements are *always recommended*:
 
- Type
- Language
- Originating File

# Example WebVTT

```
WEBVTT
Type: caption
Language: eng
Responsible Party: US, GWU/SCRC
File Creator: GWU/SCRC
File Creation Date: 2024-05-22
Originating File: rg0131_s04_ss02_c02_i04.mp4

00:01:48.000 --> 00:01:50.000
 Thank you very much.

00:01:50.000 --> 00:01:55.000
 And now we are going into our next topic.

00:01:55.000 --> 00:02:00.000
 And it's beyond the next election.

00:02:00.000 --> 00:02:08.000
 And you know the next president of the United States will be sworn in, will have been sworn in,

00:02:08.000 --> 00:02:14.000
 a year, one year, one week, and one day from now.

00:02:14.000 --> 00:02:18.000
 Not quite one day, 22 hours.

00:02:18.000 --> 00:02:29.000
 And that is a little too long to predict what, not only who he'll be and what party,

00:02:29.000 --> 00:02:35.000
 but also what the conditions are under which he will take over,

00:02:35.000 --> 00:02:41.000
 except that based on the last half, last dozen or so inaugurations,

00:02:41.000 --> 00:02:45.000
 you can predict a snowstorm in Washington for the day.
```

---
[^1]: Dave Rodriguez, Bryan J. Brown, and Florida State University Libraries, “Comparative Analysis of Automated Speech Recognition Technologies for Enhanced Audiovisual Accessibility,” The Code4Lib Journal, no. 58 (December 4, 2023), https://journal.code4lib.org/articles/17820.