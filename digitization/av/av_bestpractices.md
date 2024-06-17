---
layout: page
title: "Best Practices for Digitization (AV)"
permalink: /digitization/av_bestpractices/
grand_parent: Digitization
parent: "Digitization: Audiovisual Carriers"
nav_order: 1
---

# Best Practices for Audio and Moving Image Digitization

This is not policy, but rather a guiding document. For various reasons, projects might not be able to fulfill these recommendations. At present, technical debt related to storage and access systems makes these recommendations difficult to fulfill.

These specifications remain aspirational, but serious efforts should be made to adhere to them to better ensure the long-term preservation and usability of digitized audio and moving image material.

Additional exploration should also be conducted to explore open-source technologies like FFVI/Matroska for moving image files. 

## Audio 

### Preservation File (Master)

|       | Format          | Codec            | Bit depth + sampling                 |
| ----- | --------------- | ---------------- | ------------------------------------ |
| Audio  | Wave or Broadcast WAVE | PCM              | 24-bit bit depth; 48Hz sampling rate |

Preservation master files should represent the entirety of the source material. All intrinsic characteristics and values should be included and the complete length of the source material transferred (head to tail).

### Access File (Derivative)

| Format          | Bit rate| 
| --------------- | ---------------- | 
| MPEG-3 (MP3) | 256Kbps bit rate| 

## Moving Image

### Preservation File (Master)

|       | Format          | Codec            | Bit depth + sampling                 |
| ----- | --------------- | ---------------- | ------------------------------------ |
| Image | Quicktime (MOV) | Apple ProRes 422 | 10-bit bit depth                     |  
| Audio  | Quicktime (MOV) | PCM              | 24-bit bit depth; 48Hz sampling rate |

Preservation master files should represent the entirety of the source material. All intrinsic characteristics and values should be included and the complete length of the source material transferred (head to tail).

### Access File (Derivative)

| Format          | Codec            | 
| --------------- | ---------------- | 
| MPEG-4 (MP4) | H.264 | 

## Submission Information Packet for AV content

Digitized av content is often multiple components. These components should be packed in a single submission information packet for ingest into SCRC digital storage. 

Example SIP for a/v content:

```
ms2374_s2_c107d_f7_i1
├── ms2374_s2_c107d_f7_i1_001.mov
├── ms2374_s2_c107d_f7_i1_002.mov
└── access
    ├── ms2374_s2_c107d_f7_i1_001.mp4
    ├── ms2374_s2_c107d_f7_i1_001_eng.vtt
    ├── ms2374_s2_c107d_f7_i1_002.mp4
    └── ms2374_s2_c107d_f7_i1_002_eng.vtt
```
