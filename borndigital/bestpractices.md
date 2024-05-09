---
layout: page
title: "Best Practices for Born-Digital Accessioning: Appraisal and Migration"
permalink: /borndigital/bestpractice/
parent: Accessioning and Ingesting Born-Digital Records
grand_parent: Supporting Born-Digital Records
nav_order: 1
---

# Best Practices for Born-Digital Accessioning: Appraisal and Migration

LAI Digital Services

Draft: 2023-11-30

## Background

Quality appraisal and migration of digital records provides benefits that increase the long-term effectiveness of storage, preservation, and access. The costs of managing digital records provides incentive for practitioners to appraise records before ingestion into a repository’s digital collections when possible. Ultimately, the level of access that users can expect for born-digital records is impacted by the level of appraisal and migration afforded at the time of accessioning.

The appraisal and migration of born-digital records can not be a wholly prescriptive practice. Practitioners must make decisions throughout the process based on the context of the records, their unique characteristics, and the limitations of technology, labor, and resources at hand.

### Appraisal

Not every record has value worthy of inclusion in an archival collection. Therefore, practitioners must assess value on some level to make decisions about what to accession. To do this, the practitioner must develop an understanding of the records, the context of the creation/use, and the broader information ecosystem in which they exist. In a digital context, appraisal has similar benefits as it does with physical records. Providing long-term preservation and access to archival records has significant costs. Appraisal makes archives easier to use and manage.

It should be noted that with digital records there is often a desire to fall back on more traditional modes of appraisal. [Jenkinsonian](https://www.jstor.org/stable/40294205) inspired approaches are often taken, in part, because digital records take up no physical space. It’s perceived as easy to save everything that is transferred or offered to a repository in digital form. This is untrue. We know that these passive approaches towards appraisal accrue significant environmental, labor, and resource costs overtime. There may be value in the Jenkinsonian inspired methods for preserving [evidential value](https://dictionary.archivists.org/entry/evidential-value.html) of digital records, but the benefits are often outweighed by the costs.

### Migration

Migration encompasses the actions of acquiring, imaging, and transferring records into a repository's care. Migration may further develop the repository's understanding of the records. Decisions made during the migration process directly affect the experience that future users will have with the records.

## Decision Matrices

The below provides 3 possible scenarios that represent different levels of appraisal and migration. Practitioners might mix and match aspects of multiple levels depending on the characteristics of records and the resources available. A variety of tools, software, and hardware might be used to accomplish each task.

### Level 1. Full Migration

<table><thead><tr><th><p>Transfer</p></th><th><p>Understand/Review/Act</p></th><th><p>Documentation</p></th><th><p>Storage</p></th></tr><tr><th><ul><li>Disk image (physical media)</li><li>File Transfer</li><li>Robocopy</li><li>Virus scan</li></ul></th><th><ul><li>Search and Remediate for PII/PPI</li><li>Perform file identification and review file formats. Migrate to preferred formats as necessary</li><li>Review for bad file names or junk files.</li><li>Review files for duplicate files.</li></ul></th><th><ul><li>Create and or update ArchivesSpace accession record</li><li>Capture information about physical media.</li><li>BagIt</li></ul></th><th><ul><li>BagIt</li><li><a href="https://github.com/gwu-libraries/digital-stewardship-services">Tier 2 storage</a></li></ul></th></tr></thead></table>

### Level 2. Intermediate Migration

<table><thead><tr><th><p>Transfer</p></th><th><p>Understand/Review/Act</p></th><th><p>Documentation</p></th><th><p>Storage</p></th></tr><tr><th><ul><li>Disk image (physical media)</li><li>File Transfer</li></ul></th><th><ul><li>Perform file identification</li><li>Review for junk files</li></ul></th><th><ul><li>Create and update ArchivesSpace accession record</li><li>Capture information about physical media</li></ul></th><th><ul><li>BagIt</li><li><a href="https://github.com/gwu-libraries/digital-stewardship-services">Tier 2 storage</a></li></ul></th></tr></thead></table>

### Level 3. Base-line Migration

<table><thead><tr><th><p>Transfer</p></th><th><p>Understand/Review/Act</p></th><th><p>Documentation</p></th><th><p>Storage</p></th></tr><tr><th><ul><li>Disk Image</li><li>File Transfer</li></ul></th><th></th><th><ul><li>Create and update ArchivesSpace accession record</li></ul></th><th><ul><li><a href="https://github.com/gwu-libraries/digital-stewardship-services">Tier 2 storage</a></li></ul></th></tr></thead></table>

## Example Narratives

### Example 1. University Office transferring records to the University Archives

**Transfer**: The Office of the University President has transferred 40gb (1008 files) of records to the University Archives via file sharing platforms (Box, Google Drive, ect.) and internal systems (Office of Media Relation’s Digital Asset Management system). The University Archivist and Digital Services Manager compiled the files from various sources provided by the transferring office into a single submission information packet (SIP). A virus scan was not completed since the files previously existed solely within GWU systems.

**Understand/Review/Act:** [DROID](https://github.com/digital-preservation/droid) was used to perform file format identification. No proprietary file formats were found, therefore no file formats were migrated/reformatted. [Simple python scripts](https://github.com/DaltonAlves/GWU/tree/main/DigitalAccesioning) were run over the directory to identify files with bad file names (invalid or non-ASCII characters), 0-bit (empty) files, duplicate files, and hidden subdirectories/files. Duplicate files were reviewed by the practitioner and removed from the SIP. No bad/junk files were identified, so no further action was taken.

Through discussions with the transferring office it was determined that no restrictions apply to the records. In addition, the majority of the files were images with limited embedded metadata. Therefore, a PII search was not conducted.

The arrangement of the files as they were transferred was relatively organized and provided some eventual value related to the creation of the records, so the arrangement was maintained.

**Documentation:** An accession record was created in ArchivesSpace. The accession records include information about restriction status, extent of the accession, and the source and date of the transfer.

**Storage:** The SIP was ingested into the SCRC preservation environment as an archival information packet. The contents of the AIP are registered in an inventory by the [simple audit tool](https://github.com/gwu-libraries/audit-tool). The URI of the AIP is linked to the accession record in ArchivesSpace.

### Example 2. University Office transferring records with restrictions to University Archives

**Transfer**: The Office of the University President has transferred 4mb (50 files) of records to the University Archives via file sharing platform (Box). The files were not created nor used in the environment (Box). Therefore robocopy (or similar tools) were not used to transfer the files.

**Understand/Review/Act:** Per the University’s record retention schedule the records transferred are closed for a set period of time (50 years from date of record creation). An examination of the files indicated that the earliest file was dated 2021. Date information was appended to file names by the record creator, but in an sporadic manner. A python script was run over the files to standardize the date in the file name in YYYY-MM-DD formatting. This was done to facilitate access based upon the restriction. Spaces were also removed from file names and replaced with underscores. No PII search was conducted since the records will be closed for 50 years. A search for duplicate files was conducted and none were found.

**Documentation:** An accession record was created in ArchivesSpace. The accession records include information about restriction status, extent of the accession, and the source and date of the transfer, and the restriction. BagIt was used to package the submission information packet. This also allowed for some basic metadata related to rights to be attached to the AIP. The 50 year restriction and lack of a PII search was noted in the BagIt info file.

**Transfer:** The SIP was ingested into the SCRC preservation environment as an archival information packet. BagIt was used on the to package the SIP with relevant metadata including information about the restriction. The contents of the AIP are registered in an inventory by the [simple audit tool](https://github.com/gwu-libraries/audit-tool). The URI of the AIP is linked to the accession record in ArchivesSpace.

### Example 3. Record creator electronically transferring records as part of personal papers collection

**Transfer:** A record creator has transferred 450mb (168 files) of records as an accretion to an existing fonds. The records were transmitted via a file sharing platform (Box). A virus scan was completed on the files before ingestion into GW systems. Robocopy was not used because no physical media was used during the transfer and files were not used nor created by the record creator in the environment in which they were transferred.

**Understand/Review/Act:** Through discussions with the record creator and examination of the files it was understood that the files were not systematically arranged by the record creator. Rather, they were accumulated over-time in a file sharing platform in an unorganized and inconsistent manner. NARA’s [Electronic Records Accessioning Support Tools](https://github.com/usnationalarchives/Electronic-Records-Accessioning-Support-Tools) were used to identify file formats, duplicate files, and to search for “funny” file names (non-ASCII characters). Many files were present in multiple file formats. For example, PDFs and text documents (.pages) containing the same content. Pages files are a proprietary document format supported only on Apple devices. To facilitate future use, unique pages files (files with no PDF extant equivalent) were migrated to the PDF/A file format. Duplicate files were not retained once it was confirmed that they existed in another preferred file format (PDF/A).

Some arrangement was carried out to better structure the files after consultation with the record creator. Files were organized to be more consistent in a hierarchical structure (grouping together project files, organizing correspondence into subdirectories, ect).

Documentation: An accession record was created in ArchivesSpace. The accession record includes information about restriction status, extent of the accession, and the source and date of the transfer.

**Storage:** the SIP was ingested into the SCRC preservation environment as an archival information packet. The contents of the AIP are registered in an inventory by the [simple audit tool](https://github.com/gwu-libraries/audit-tool). The URI of the AIP is linked to the accession record in ArchivesSpace.

### Example 4. Physical Media transferred with non-digital records

Transfer: A record creator has transferred 2 linear feet of records as an [accretion](https://dictionary.archivists.org/entry/accretion.html) to an existing fonds. Within this material are physical media carriers containing born-digital records. A virus scan of the physical media was performed. Robocopy was used to migrate the files off of the physical media to retain file and folder attributes (timestamps, ownership information, and other attributes). A write-blocker device was used when handling the digital files on the physical media carriers.

**Understand/Review/Act:** The physical media devices contained less than 1mb of data in about 20 files across approximately 10 media carriers (3.5 IN floppy discs). The files on each floppy did not contain file extensions (file formats), but upon closer examination they were identified as plain text files. The physical media did contain important contextual and descriptive information. This information was used in the archival description. It was decided not to photograph the physical media since the media would be retained within the collections. Unlike previous examples, the review of these files was done via mostly manual means because of the simplicity of the files and the amount of files.

**Documentation:** The accession record was updated to reflect the information learned about the digital files: the extent (size and # of files) and dates (from the original timestamps).

**Storage: The original files without file formats and migrated file formats (.txt files) were ingested as a single SIP.** The contents of the AIP are registered in an inventory by the [simple audit tool](https://github.com/gwu-libraries/audit-tool). The URI of the AIP is linked to the accession record in ArchivesSpace.

## Thoughts for the Future

While many appraisal and migration activities require the expertise of archivists and other practitioners the overall process leverages many tools that make the process scalable. These tools should be further explored to identify what works best for the needs of LAI and is usable given the available resources and skill sets of staff.

Packaging of tools as microservices in a broader system to support digital accessioning has many benefits. Examples of these types of services include: [Archivematica](https://www.archivematica.org/en/), [Aurora](https://github.com/RockefellerArchiveCenter/aurora) (and the broader [Project Electron](https://github.com/RockefellerArchiveCenter/project_electron)), [FITS](https://projects.iq.harvard.edu/fits), [Preservica](https://preservica.com/), and [BitCurator](https://bitcurator.net/).

In addition, ArchivesSpace and BagIt info files are currently the only available resources for recording and storing important administrative and preservation metadata information for AIPs. ArchivesSpace (and Encoded Archival Description) as a system of record is not ideal for these types of metadata. LAI’s digital stewardship program does not presently support broader use of XML-based metadata for management of digital objects outside of EAD.

Further exploration of packaged microservices and more robust support for metadata is crucial as the scale and complexity of digital accessions increases.