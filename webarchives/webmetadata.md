---
layout: page
title: "Metadata for Web Archives"
permalink: /webarchives/metadata/
parent: GW Web Archives
---

# Metadata for Web Archives

Metadata for web archives exists in two primary places: within Archive-It, the system used by GWLAI to collect and manage its web archives collection, and within ArchivesSpace, the system that GWLAI uses to describe its archives collections.

Archive-It uses 15 Dublin Core elements. Additional custom metadata fields may also be applied. These metadata fields may be applied to any level of a web archive: collection, seed, and document. SCRC primarily applies metadata to the collection and seed level. See the [Add, edit, and manage your metadata article](https://support.archive-it.org/hc/en-us/articles/208332603-Add-edit-and-manage-your-metadata) in the Archive-It Help Center for more information about metadata and Archive-It

This page synthesizes local application recommendations based upon the *Descriptive Metadata for Web Archiving: Recommendations of the OCLC Research Library Partnership Web Archiving Metadata Working Group.* [^1]

## Metadata Profile for Web Archives

| Element                | **Required/Optional** |
| ---------------------- | --------------------- |
| [Title](#title)        | **Required**          |
| [Description](#description) | **Required**    |
| [Collector](#collector) | **Required**         |
| [Date](#date)          | **Required**          |
| [Language](#language)   | **Required**         |
| [Creator](#creator)    | **Strongly Encouraged**        |
| [Identifier_Collection](#identifier_collection) | **Strongly Encouraged** |
| [Subject](#subject)    | **Strongly Encouraged**   |
| [Source of Description](#source-of-description) | **Optional** |
| [Genre/Form](#genreform) | **Optional**        |
| [Contributor](#contributor) | **Optional**     |

This metadata profile is primarily designed for individual seeds within web archive collections, rather than entire collections of web archive content. While it shares similarities with metadata used in finding aids/EAD, it focuses specifically on metadata creation for individual seeds.

Metadata should be applied to seeds in Archive-It when they are created. It is *strongly encouraged* that all new seeds receive all *required* fields from this profile.

### Title

| **Required**        | Explanation                                                                                                                          |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| Definition                   | The name by which an archive website or collection is known.                                                                         |
| Standard Usage for SCRC      | Office of the President website                                                                                                      |
| Standards                    | DACS 2.3                                                                                                                             |
| Guidance                     | Transcribe directly from the head of the homepage (website) or inspect the homepage for a relevant metatag or other related element. |

### Description

| **Required**        | Explanation                                                                                                                                                                |
| ---------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Definition                   | One or more notes explaining the content, context, and other aspects of an archived website or collection.                                                                 |
| Example Usage for SCRC       | Website of the Office of the President, George Washington University. Contains information about the President’s office and community messages published by the President. |
| Standards                    | DACS 3.1                                                                                                                                                                   |
| Guidance                     | Briefly describe the scope and content of the archived website. Describe what the website is about, its purpose, and describe who created it.                             |

### Collector

| **Required**     | Explanation                                                                                                                                                            |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Definition                   | Organization responsible for collecting the archived content.                                                                                                          |
| Example Usage for SCRC       | - Special Collections Research Center, The George Washington University<br> - George Washington University Libraries                                                        |
| Standards                    | DACS 2.2                                                                                                                                                               |
| Guidance                     | Identify the institution responsible for selecting websites for archiving, crawling the websites, and creating and maintaining the metadata that describes the content |
| Note                         | Use SCRC when content falls under SCRC collecting scope. Use GW Libraries when content falls outside of SCRC collecting scope.                             

### Date

| **Required**        | Explanation                                                                                                                                                            |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Definition                   | A single date or span of dates associated with the _capture_ of an archived website or collection.                                                                                                       |
| Example Usage for SCRC       | * Date first crawled: 2024-11-01<br>* Captured 2024-ongoing<br>* Captured 2021-2024                                                                                                                        |
| Standards                    | DACS 2.4                                                                                                                                                              |
| Guidance                     | For non-scheduled crawls, use single dates. For seeds that are scheduled, use an ongoing date. If a scheduled seed becomes inactive, use an end date as part of a date range.                             |
| Note                         | Do not include dates outside the range of the archived content. For example, if a website was first crawled in 2024, but the website was initially created in 2004, only use the 2024 date.              |

### Language

| **Required**        | Explanation                                                                                                                      |
| ---------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| Definition                   | The language(s) of the archived content.<br>                                                                                      |
| Standard Usage for SCRC      | English<br>Spanish<br>Chinese                                                                                                        |
| Standards                    | DACS 4.5                                                                                                                         |
| Guidance                     | This field may be repeated as many times as necessary to capture the languages used throughout the archived content.<br>Use the English name of Language from ISO 639.2 (not the ISO codes) |

### Creator

| **Strongly Encouraged**        | Explanation                                                                                                                                                                                                                                           |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Definition                   | An organization or person principally responsible for creating the intellectual content of an archived website or collection.                                                                                                                         |
| Standard Usage for SCRC      | George Washington University. Office of the President                                                                                                                                                                                                 |
| Standards                    | DACS 2.6                                                                                                                                                                                                                                              |
| Guidance                     | The creator of a single website, such as an institutional home page, blog or twitter feed, usually is easily identified unless purposely anonymous, while a collection of websites focused on a current event or topic rarely has an overall creator. See also: [contributor](#contributor).|

### Identifier_Collection

| **Strongly Encouraged**        | Explanation                                                                                              |
| ---------------------------- | --------------------------------------------------------------------------------------------------------|
| Definition                   | The collection Identifier associated with the archived website. Use the resource record that                                                 |
| Example Usage for SCRC       | - RG002<br> - MS2285<br> - NEA1011-RG                                                                                    |
| Standards                    | DACS 2.1                                                                                                 |
| Guidance                     | Identify the creator of the website first, then see if there is a collection for that creator.           |
| Note                         | May use multiple collection identifiers if the archived website is associated with multiple collections. |

### Subject

| **Strongly Encouraged**        | Explanation                                                                                                                                                                                                    |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Definition                   | Primary topic(s) describing the content of an archived website or collection                                                                                                                                   |
| Example Usage for SCRC       | \- George Washington University<br>\- Education, Higher -- United States<br>\- Cross-country running                                                                                                           |
| Guidance                     | Identify the creator of the website first, then see if there is a collection for that creator.                                                                                                                 |
| Note                         | Identify topical subjects, geographic locations, and people and organizations relevant to the content of the collection.<br>Use subjects already present in ArchivesSpace. If not present, use FAST or LCSH.    |

### Source of Description

| **Optional**        | Explanation                                                                                                                                |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| Definition                   | Information about the gathering or creation of the metadata itself, such as sources of data or the date on which source data was obtained. |
| Example Usage for SCRC       | Description based on archived webpage captured on November 6, 2024.                                                                        |
| Standards                    | DACS 7.1.8        |
| Guidance                     | Added value. Use when the website has been crawled for a long period of time and undergone many changes.                                   |

### Genre/Form

| **Optional**        | Explanation                                                                                                                                 |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Definition                   | The type of content in an archived website or collection.                                                                                   |
| Example Usage for SCRC       | \- Website<br>\- News article<br>\- Social Media                                                                                            |
| Note                         | At present, do not use for individual seeds/websites unless the format is uncommon. This is mostly relevant to collection-level metadata or description for web archives in ArchivesSpace (finding aids). |

### Contributor

| **Optional**        | Explanation                                                                                                                                                                                                                                           |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Definition                   | An organization or person secondarily responsible for the content of an archived website or collection                                                                                                                                                |
| Example Usage for SCRC       | Knapp, Steven, 1951-                                                                                                                                                                                                                               |
| Standards                    | DACS 2.6                                                                                                                                                                                                                                              |
| Guidance                     | If two or more entities share principal responsibility, place them all in Creator field. Otherwise, place one in the Contributor element. *Use Contributor for all that have secondary responsibility*                                        |
| Note                         | Use agent records from ArchivesSpace. If agent record not present, please reach out to the archivist responsible for the relevant collection area to discuss adding an agent record. When no agent record is present in ArchivesSpace, use LCNAF.<br> |

[^1]: Dooley, Jackie, and Kate Bowers. 2018. Descriptive Metadata for Web Archiving: Recommendations of the OCLC Research Library Partnership Web Archiving Metadata Working Group. Dublin, OH: OCLC Research. https://doi.org/10.2
