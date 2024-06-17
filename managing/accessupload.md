---
layout: page
title: "Access Upload - InternetArchive"
permalink: /managing/accessupload/
parent: Managing Digital Collections - Access and Preservation
---
# Uploading and Ingesting Digital Collections to Access Systems
Presently, GWU Special Collections only ingests access copies of digital collections materials into Internet Archive. In the past, some digital collection material was ingested into GW ScholarSpace, the institutional repository, managed by GW LAI. 

## Uploading Digital Collections to Internet Archive
### Resources
- [Internet Archive Metadata Documentation](https://archive.org/developers/metadata-schema/index.html) 
- [Internet Archive Python Library](https://archive.org/developers/internetarchive/)
- [Internet Archive File Formats](https://help.archive.org/help/file-formats/)
- [Internet Archive File Derivatives](https://archive.org/help/derivatives.php)
- [Internet Archive OCR](https://archive.org/developers/ocr.html)
  
### Supporting Documents
- [GW SCRC Metadata Scheme for Internet Archive (Documents and Text)](/assets/files/MetadataScheme_GWSCRC_Documents.xlsx)
- [GW SCRC Metadata Scheme for Internet Archive (Moving Images and Audio)](/assets/files/MetadataScheme_GWSCRC_AudioVideo.xlsx)
- [Example Upload CSV - Documents and Text]()
- [Example Upload CSV - Moving Images and Audio]()
  
### Installing internetarchive python library
- Follow [the directions and documentation provided by the InternetArchive](https://archive.org/developers/internetarchive/installation.html).
  - If you already have python installed you may be able to just use ['pip install internetarchive'](https://pypi.org/project/internetarchive/)
  
### Preparing to upload content to Internet Archive
- Generally, we only submit derivative access copies to Internet Archive. Therefore, if you haven't already you will need to prepare access copies from your master files.
- In the same directory as your access copies, create a CSV modeled on the *GW SCRC Metadata Scheme for Internet Archive* (see above) to hold the metadata for each record.
- You may use the [ArchivesSpace_to_InternetArchive script]() to generate metadata from the archival description for each record. 
  - If you use this script, you should still review the metadata before upload. The script pulls description from ancestor records (series, resource, ect.) that may not be appropriate for what is represented by the digital content.
    - An example of this might be rights information. The script will pull the rights statement from the resource (collection) record. This may not apply to item-level description for the digital content.
- You may also include additional derivatives (SRT/VTT caption files, full text txt files) in your upload. To do so, add an additional row to the CSV for each identifier. Match the identifier to the file of the additional derivative. 
![CSV screenshot](/assets/images/sidecar_upload.png)

### Uploading Content to Internet Archive
- Once both your files and metadata are prepared you are ready to upload! To do so, you can use your command line interface to start the upload. In your command line (PowerShell, Terminal, ect.) navigate to the directory with the files and your CSV spreadsheet. 
  - Tip: On Windows, you can open PowerShell from the file explorer to skip navigating to the directory via the command line.
- Run the following, where "uploading.csv" is switched out for the name of your metadata CSV: 
> ia upload --spreadsheet=uploading.csv

### Describing online digitized content in finding aids
We use [digital archival objects](/daos/) in ArchivesSpace to connect archival description to digitized content. The digital archival object records points users to digital content outside of ArchivesSpace. Digital archival objects can also allow digital content to be displayed alongside archival object description. 

After uploading content that was digitized from archival collections you must create digital archival objects. To do so, see [digital archival objects](/daos/),