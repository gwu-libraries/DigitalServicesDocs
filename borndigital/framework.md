---
layout: page
title: "Framework for Born Digital Accessioning"
permalink: /borndigital/framework/
parent: Supporting Born-Digital Records
parent: Accessioning and Ingesting Born-Digital Records
grand_parent: Supporting Born-Digital Records
nav_order: 2
---
#  Framework for Born-Digital Accessioning & Appraisal

Updated: 2023-11-01

## Scope

Transfer of digital records related to [specialized collections](https://dictionary.archivists.org/entry/special-collection.html) into the care of GW Libraries & Academic Innovation. This primarily relates to born-digital records, but may also apply to digital surrogates that are transferred to GWLAI as digital records. This framework does not apply to digital surrogates produced by GWLAI.

**Purpose and Goals:**

_Digital accessioning_ activities should strive to maintain the [archival integrity](https://dictionary.archivists.org/entry/archival-integrity.html#.V1caG_krLiw) of digital records while preparing them to be ingested into a digital preservation environment.

_Digital appraisal_ activities encompass both [the selection of digital records](https://dictionary.archivists.org/entry/appraisal.html) and the assurance that these records adhere to LAI’s digital preservation best practices.

Some goals of these activities include:

- Gather information before acquisition (if possible)
- Transfer materials to institution
- Identify and appraise media carriers
- Scan content for viruses/malware
- Identify temporary files and artifacts and software that is unwanted or unneeded
- File identification and format characterization
- Analyze for sensitive content
- Analyze for technical metadata
- Create/extract digital object metadata
- Assemble AIP and DIP
- Transfer AIP to preservation environment
- Create base-line documentation in ArchivesSpace (accession record)
- Use documentation and information generated from accessioning and appraisal to inform an initial processing plan

## Narrative

### Gather Information before Acquisition

Pre-appraisal of digital materials should be conducted when possible. These pre-appraisal activities will guide decision-making related to the acquisition and transfer of digital records. They may also impact future preservation and access actions.

Discussions with donors and record-creators should be conducted to produce documentation about media devices or files, the transfer process, and the shared vision between archivist and record creator regarding the preservation and access of the digital collections materials.

Discussion points include:

- Access restrictions (copyright, privacy, ect)
- Permission to crawl related networked and or web-based materials (Web crawling or scrapping of networked systems).
- Copyright

_This step is recommended._ In some cases, digital records have already been transferred to LAI and it may be difficult or impossible to gather this information.

### Transfer Materials to Institution

Digital records may be transferred via web-based file transfer tools or via physical media devices.

For physical media transfers, the physical carriers should be identified and appraised to identify media that does not need to be copied (duplicates, out-of-scope material, ect.). Disk images for physical media will be created.

All digital files will be copied to a temporary staging location.

_This step is mandatory_. The transferred files constitute the SIP in the [OAIS reference model](https://dictionary.archivists.org/entry/open-archival-information-system.html).

### Virus Check

For digital records stored on physical media devices, the virus check should be conducted before transfer to the temporary staging location. A write blocker must be used when conducting the initial virus check. For files transferred wholly via digital methods, the virus check will take place from the temporary staging location or if possible before transfer to LAI (conducted with the donor).

In the event of infected items the entire image might be quarantined or specific infected files might be discarded.

_This step is recommended._

### File Identification and Format Characterization

Format characterization and file identification should be conducted to better understand the deposited material. This information will be used to guide future preservation efforts for the individual deposits, but also guide the overarching preservation strategy of the repository.

This is especially important for born-digital content in which the diversity of file formats make preservation difficult past bit-level preservation. File and format analysis allows for aggregated decision making about functional-level preservation.

File identification and format characterization is also used to create metadata that may be used during the processing of digital records.

_This step is recommended._

### Analyze for Sensitive Content

This step should build on information that was acquired during the pre-acquisition stage, if possible. Manual review of digital files may be possible for small deposits of records, but digital forensic tools should be used when possible. Manual reviews may neglect to find hidden or obscured sensitive content that could be embedded in files or file systems past the surface level.

Sensitive Content may include records that were unintentionally transferred through human error or unknowingly through deleted or hidden files.

_This step is recommended._

### Establish Fixity

Fixity information is important provenance information that ensures the integrity of the records. In certain circumstances, fixity should be established prior to ingestion into a digital preservation environment. Fixity information may be used to demonstrate successful transfer of files from record creator to the repository.

Once ingested into the preservation environment records are regularly checked for fixity using GWU LAI’s [Audit Tool](https://github.com/gwu-libraries/audit-tool).

This step is mandatory. It is up to the archivist (record custodian) to decide when and how fixity is established. In most cases, fixity will be established when the AIPs are assembled. In some cases checksums may be generated earlier.

### Assemble AIP

The Archival Information Package is a collocation of the deposited records and any information gathered during the previous steps. This is the information package that is ingested into the preservation environment.

_This step is mandatory._

### Assemble DIP

The Dissemination Information Package is the access copy of the AIP. DIPs should, when possible, include enhancements like closed captions, alt-text, and sound/image quality improvements.

DIPs may be served to patrons via digital access systems and repositories, but they may also be served on an ad-hoc basis. In an ad-hoc scenario, the DIP may not be assembled ahead of time.

_This step is not mandatory, but in many cases recommended._ If a DIP isn’t assembled we can assume the digital objects are in a [dark environment](https://dictionary.archivists.org/entry/dark-archives.html) without public access.

### Create Baseline Accession Record

Accession records provide baseline documentation about digital objects’ acquisition and provenance. Information recorded should be related to: titles, accession numbers, date of material created, extent, copyright information, and processing status.

_This step is mandatory._ Digital records may be covered under pre-existing accession records and or accession records that include non-digital records.

## Potential Tools/Resources to Explore

All of the below are open source tools unless noted otherwise

| Tool/Resource | Scope | Notes |
| --- | --- | --- |
| [DROID (National Archives, UK)](https://github.com/digital-preservation/droid) | File Identification and Format Characterization | Has GUI; support for linux, windows, osx |
| --- | --- | --- |
| [Bagger (LoC)](https://github.com/LibraryOfCongress/bagger) | AIP creation | JAVA GUI and python library. JAVA GUI is possibly being phased out (LC releasing more info soon).<br><br>Started to outline an example [bagger profile](https://docs.google.com/document/d/1T_0A55HRgT1tUwntSo7Ple78SYXM_6R-LJg4SQgfmUc/edit?usp=sharing). This could be used with Bagger GUI/python OR Baggit Java library. |
| --- | --- | --- |
| [Exactly (AVP)](https://github.com/WeAreAVP/uk-exactly) | AIP creation and transfer to preservation environment | Bags and FTP transfer; also supports getting records transferred from record creators |
| --- | --- | --- |
| [Bulk_extractor](https://github.com/simsong/bulk_extractor) | Forensic analysis for PII/PPI |     |
| --- | --- | --- |
| [Audit Tool](https://github.com/gwu-libraries/audit-tool) | Fixity check, inventory and monitoring. | Currently in use on LAI digital specialized collections material. |
| --- | --- | --- |

Below are applications that contain many microservices including some of those listed above.

| Tool/Resource | Scope | Notes |
| --- | --- | --- |
| Archivematica |     |     |
| --- | --- | --- |
| BitCurator | Disk imaging; file identification and format characterization; technical metadata extraction; forensic analysis for PII/PPI; AIP packaging | Deployed on Ubuntu VM. Supports PREMIS records. There was support for Aspace integration – no longer actively developed. |
| --- | --- | --- |
| [FITS (Harvard)](https://projects.iq.harvard.edu/fits) | Identifies, validates, and extracts technical metadata for a wide range of file formats.  <br><br/>Wrapper for a variety of open source tools. | Contains: Apache Tika, JHove, MediaInfo, Exiftool, National Library of New Zealand Metadata Extractor, DROID, FFIdent, File Utility<br><br>Command line and API |
| --- | --- | --- |
| FTK Imager | Disk imaging; Forensic analysis; some content analysis | **Proprietary.** |
| --- | --- | --- |
| Hyrax | File Information Tool Set (FITS) tool for technical metadata. Fixity via Fedora |     |
| --- | --- | --- |
