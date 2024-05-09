---
layout: page
title: "Digitization - File Names"
permalink: /digitization/filenames/
parent: Digitization
---
# File Naming Conventions

## General Rules
- Be consistent in your file naming for a project. Look at past related projects to help determine a structure for file names. Consistency within and across projects will allow for easier management and manipulation of files.
- Use leading zeroes when necessary. Never use a single digit without a leading zero.
    - "1" = bad
    - "01" = good
  
## Suggested and Example File Name Structures

These are suggested file names. Depending on your project there may be valid reasons to deviate from these structures.

### Manuscript/Archival Material
- ms####_s##_c##_f##_i##_p###
- Breakdown of elements:
  - ms = collection identifier
  - s = series
  - c = container (ignore the container type indicator in ArchivesSpace, use "c" regardless of type)
  - f = folder
  - i = item
  - p = page
- Example = ms2123_s11_ss01_c31_f01.pdf


### File names for materials from Corcoran Archives
For materials from the Corcoran Archivces collections following structure should be used.

#### Collection IDs
The collection identifier should be simplified as follows:
 - COR0001.0-RG -> cor1-0
 - COR0003.1-RG -> cor3-1
 - COR0013-MS -> cor13
  
#### Containers

Container numbers should be simplified as follows:
- Box RG2-2008.018 -> rg2-2008-018
- Box RG5.0-2008.029 -> rg5-0-2008-029

#### Full file name examaples:
cor2-0_s01_ss01_rg2-2008-001_f11_i01.tiff
cor5-0_s06_ss01_rg5-2008-020_f01.pdf
  
### Cataloged Books & Pamphlets (rarebooks)
- CallNumber_PageNumber
  - Example = spec_ps3544_h56_page34.tif
  - 'spec' may be replaced with other collection areas depending on call number in catalog (ex. mei, kiev)

### Serials (cataloged and from manuscript collections)
In general, it is best to create file names for serials that reflect the items' volume/sequential designation (ex. vol. 1, no. 1). For serials that exist within an archival collection, this information can be easily confused with the top container type "volume." Therefore, the volume designation of the actual work should be used over the instance record volume. 

Example:
- RG0044_s39_vol12_no03
- GWNews_vol12_no03

It is also appropriate to use date information to form file names. This may be relevant if the volume/sequential designations are not present or irregular. 
- FBNews_1965_10

Example:
- GWNews_199712 (Title_YYYYMM)
- GWTimes_199712-199801 (Title_YYYMM-YYYYMM)
  
### Audiovisual Material
In certain cases, an audiovisual work may have multiple parts. Maintaining consistency within the project and including as much collection identifying information as possible is essential.

In addition, audiovisual material is often minimally described and processed in an archival collection. Often a single archival object may represent many audiovisual items. 

Examples of file names:
- collectionID_s#_c#_f#_i#
- collectionID_s#_c#_title_of_video
- collectionID_c#_title_of_video 
- collectionID_s#_c#_f#_i#_part1
- CollectionID_c#_title_of_video_part2

### Born Digital Material
While this section is specifically for filenaming conventions used for digitized content, it should be mentioned that it is often inappropriate to change file names of born-digital records. The original file names, as given by the record creator/s, should be respected when possible. Normalization of born-digital file names can be done (removing bad characters, spaces, ect), but it is not recommended to try to make them fit any of the above schemes. 