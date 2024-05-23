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
WebVTT files should inherent the file name of the AV source file. The file name should also include information about the language and WebVTT type to improve accessibility.

Example:
- *Source AV File*: ms0000_s01_ss02_c03_i01.mp4
- *WebVTT Type*: caption
- *Language*: eng
- **WebVTT file**: ms0000_s01_ss02_c03_i01.caption.eng.vtt

# Metadata for WebVTT 
See [Guidelines for Embedding Metadata in WebVTT Files (FADGI)](https://www.digitizationguidelines.gov/guidelines/accessibilty_WebVTT.html). Required elements should be used when possible. The following elements are *always recommended*:
 
- Type
- Language
- Originating File

---
[^1]: Dave Rodriguez, Bryan J. Brown, and Florida State University Libraries, “Comparative Analysis of Automated Speech Recognition Technologies for Enhanced Audiovisual Accessibility,” The Code4Lib Journal, no. 58 (December 4, 2023), https://journal.code4lib.org/articles/17820.