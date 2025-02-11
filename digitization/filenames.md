---
layout: page
title: "Naming and Organizing Digital Surrogate Files"
permalink: /digitization/filenames/
parent: Digitization
nav_order: 1
---
# Naming and Organizing Digital Surrogate Files

Prior to actually starting any digitization project you should decide on a structure and scheme for organizing and naming the files you produce. 
  
## Using RefIDs for File Names

For material that is represented in ArchivesSpace by a corresponding archival object record, the **refid** of the record should be used the basis of the file name and organization.  

Start by creating a directory (folder) with the refid as the name. Any files that you produce should use the refid as the basis of the file name.

### Example: 2-sided cassette

```
root_folder/
├── ref9916/
  ├── ref9916_001.wav
  ├── ref9916_002.wav
  └── derivatives/
      ├── ref9916_001.mp3
      ├── ref9916_001_caption_eng.vtt
      ├── ref9916_002.mp3
      └── ref9916_002_caption_eng.vtt
```

### Example: text-based document
```
root_folder/
├── e203d9a24f90f062871a72fe359c7900/
  ├── e203d9a24f90f062871a72fe359c7900_001.tif
  ├── e203d9a24f90f062871a72fe359c7900_002.tif
  ├── e203d9a24f90f062871a72fe359c7900_003.tif
  ├── e203d9a24f90f062871a72fe359c7900_004.tif
  ├── e203d9a24f90f062871a72fe359c7900_005.tif
  ├── ...
  └── derivatives/
      └── e203d9a24f90f062871a72fe359c7900.pdf
 ```

## Born Digital Material
While this section is specifically for conventions used for digital surrogates, it should be mentioned that it is often inappropriate to change file names of born-digital records. The original file names, as given by the record creator/s, should be respected when possible. Normalization of born-digital file names can be done (removing bad characters, spaces, ect), but it is not recommended to try to make them fit any of the above schemes. 