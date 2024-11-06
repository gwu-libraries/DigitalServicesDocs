---
layout: page
title: "SCRC Digital Collection Storage"
permalink: /managing/storage/
parent: Managing Digital Collections - Access and Preservation
---

# SCRC Digital Collection Storage

SCRC digital collections are presently stored and managed within Amazon Web Services' "Simple Storage Service (Amazon S3)." This cloud-based storage environment is used to maintain Archival Information Packages (AIPs).

## DigCol Cloudfront Application
[Digcol-cloudfront-app Repo](https://github.com/gwu-libraries/digcol-cloudfront-app) 

For internal access to SCRC Digital Collections Storage and the AIPs that it contains, SCRC staff may browse an inventory of the storage environment via the DigCol Cloud Front application. This tool provides direct access to AIPs and facilitates the retrieval of digital content.[Digital Archival Object records](/managing/daos.md) are leveraged to maintain URIs that link Archival Objects with their corresponding digital content in the SCRC Digital Collections Storage, accessible through the DigCol CloudFront application.

Access to the cloudfront application requires authentication via GW Single Sign-on.

## Technical Debt

Historically, SCRC has not packaged digital collection objects with metadata. This absence of descriptive, administrative, and technical metadata presents significant challenges for managing and providing access to digital collection materials. Without this critical information, it becomes more difficult to ensure the proper organization, preservation, and discoverability of digital objects, potentially hindering long-term access and curation efforts.