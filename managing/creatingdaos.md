---
layout: page
title: "Creating Digital Object Records"
permalink: /creatingDAOS/
parent: Digital Objects - ArchivesSpace
grand_parent: Managing Digital Collections - Access and Preservation
nav_order: 1
---

These instructions are a work in progress. Efforts are underway to integrate the creation of digital object records within broader workflows. These new workflows would generate digital object records upon ingest into the preservation environment or access systems.

# Using Digital Object Creator (Google Colab Notebook)
[Aspace Digital Object Creator](https://drive.google.com/drive/folders/1br8rcrGZlsoAOBGiLDVIG12c8szJwXuQ?usp=drive_link)

Digital object records may be created using the above Google Colab notebook. This notebook creates digital object records and links them to their associated archival object records via the ArchivesSpace API.

## CSV setup
+ new title (optional) = If this field is left blank, the title of the digital object will be inherited from the linked archival object. You can use this field if you'd like the title to be different from the archival object. 
+ file_uri = the URI of the related digital object. For preservation copies, this should point to the location on the SCRC preservation server. For access copies, the URI is the link to the digital object in a digital repository.
+ archival_object_source = the URL of the archival object which the digital object record will be linked to. This AO link can either be from the PUI or staff interface.
+ publish_link = set FALSE for preservation copies; set TRUE for access copies. This "publish" refers the publication status of the URI in the DO record. It does not refer to if the DO record itself is published.
+ xlink_actuate_attribute = "onLoad" (don't change this)
+ xlink_show_attribute = "new" (don't change this)


## Digital Objects for Access Copies (public access)

Digital object records may be used to link an archival object to a digital instance within an access system. In our current environment, this would most likely be content hosted in InternetArchive or GW ScholarSpace.

The digital object record should be published and the URI to the digital content should also be published.

Digital object records, created via the Digital Object Creator will get "Online Copy:" appended to the title of the digital object record.

## Digital Objects for Preservation Copies (dark archives)

Digital object records may be used to link an archival object to a digital instance within the SCRC preservation environment. This digital content might represent the master files associated with digital content or other digital files that have not been made publicly accessible.

The digital object record should be published, *but* the URI to the digital content *should not* be published.

Publishing the digital object record serves to alert users to the existence of the digital content, but the URIs to the SCRC preservation environment are not meant for public use -- and are inaccessible without proper permissions. 

Digital object records, created via the Digital Object Creator will get "Preservation Copy:" appended to the title of the digital object record.