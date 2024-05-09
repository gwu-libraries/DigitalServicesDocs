---
layout: page
title: "Quickguide: Born-Digital Record Accessioning"
permalink: /borndigital/guide/
parent: Accessioning and Ingesting Born-Digital Records
grand_parent: Supporting Born-Digital Records
nav_order: 3
---

# Quick Guide: Born-Digital Record Accessioning

Updated: 2024-01-04

This guide is for digital records that have not been accessioned nor processed. This workflow does not necessarily apply to digital records already processed within an existing collection. This workflow does not discuss description of digital records. It is limited to the accessioning and subsequent ingestion of records into the digital preservation environment.

Part 1 is to be carried out by the processing archivist.

Part 2 is to be carried out by the processing archivist and the Digital Services unit.

Parts 3-4 are to be carried out by the Digital Services unit.


## Part 1 - Create Baseline Documentation and Notify Digital Services

### Step 1 - Create a Baseline ArchivesSpace accession record

This accession record may also include physical records.

Estimate extent of digital content. This doesn’t need to be in terms of actual data (ex. 50 gigabytes, 1235 files, ect), but can be more abstract. For example, you can provide an estimate of the number of physical media carriers or the number of file transfers performed.

Record information about transfer/provenance: Where did the files come from? How were they acquired?

Include information about relevant restrictions or possible privacy concerns.

### Step 2 - Create an item for the accession on the [SCRC Accessions](https://gwlai.monday.com/boards/922338846) Monday board

### Step 3. Toggle the appropriate option for the “Digital Content?” field

This will automatically notify the Digital Services unit of the digital content and place an item on [the Born-Digital Record Ingestion board](https://gwlai.monday.com/boards/4927199514).

### Step 4. Provide content to Digital Services unit

For physical media (harddrives, usb drives, legacy media, ect), you can provide the media carriers to the digital services unit. For records that were transferred electronically (via Box, Google Drive, email, ect) you can share the relevant links with the digital services unit. Some of this information can be tracked using comments on the Monday board.

## Part 2 - Appraisal

### Step 5. Appraise records to create a preliminary plan for what to ingest

Not all records transferred to the repository will be ingested. Minimal appraisal of records should be completed before ingestion when possible.

The digital services unit will create additional documentation that can be used to better understand the digital records. These file reports will provide basic metadata about file names, formats, sizes. Tools can also be used to identify duplicate or unwanted files and files that may contain PII/PPI.

## Part 3 - Ingest: Transfer and Migration

### Step 6. Transfer digital records into a temporary staging area

### Step 7. Carry out actions outlined in the preliminary plan

Image and transfer digital records off of original physical media carriers. This might include deleting unwanted files, removing duplicates, standardizing file names, ect.

### Step 8. Create Submission Information Package

Package the files into a single submission information package. This SIP will be ingested into the preservation environment as the archival information package. BagIt may be used to package the SIP.

### Step 9. Ingest into Preservation Environment (preservation server)

See uploading to preservation environment documentation

## Part 4 - Update baseline documentation

### Step 10. Create digital object in Archivesspace

The AIP in the preservation environment should have a corresponding digital object in Archivesspace where the URI of the AIP is linked as a file version in the digital object record.

**Required fields:**

- **Title:**
  - Briefly describe the files (ex. Local Union #190 meeting minutes, MS2012 DiskImage #1, 2024 Granberg Inauguration Photographs)
- **Identifier:**
  - Use the accession number, include “Accession_” (ex. Accession_2024-001, Accession_2023-021)
- **File Version:**
  - URI pointing to the AIP

Publish the DO record, but do not publish the file version URI.

### Step 11. Link Digital Object to Accession Record

The new digital object (with URI to the AIP) should be linked to the existing accession record as an instance.

### Step 12. Update Accession Record with any additional information gathered

For example, a more exact extent may now be included in the accession record. Any actions carried out on the records may also be noted in the accession record.