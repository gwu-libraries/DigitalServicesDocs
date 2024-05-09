---
layout: page
title: "Digital Objects - ArchivesSpace"
permalink: /daos/
parent: Managing Digital Collections - Access and Preservation
has_children: true
---
## Digital Objects in ArchivesSpace

Digital object records in ArchivesSpace are used to link archival object records to their digital manifestations. A Digital object in ArchivesSpace is an *instance record.* 

Digital object records are encoded in EAD as [*digital archival object* elements](https://www.loc.gov/ead/EAD3taglib/EAD3-TL-eng.html#elem-dao). EAD defines a DAO as: 
"A child element of < did > used for linking to born digital records or a digital representation of the materials being described"

## Background

When locating physical materials, we use two types of records (top level containers and locations) to locate non-digital materials. The top level containers define the real-world objects that staff pick up, move, store, ship, and otherwise locate and handled in the real world. A top level container is a type of what ArchivesSpace calls an “instance”. Aspace offers two types of instances:
- top level container
- digital object

In the same way that we use top level containers and location to locate non-digital materials, we use ***digital archival objects*** to locate digital materials. Digital objects define the primary objects that staff move, store, copy, verify, track, and otherwise locate and handle in the digital world. A digital object is treated as the equivalent of a top level container. The two have one significant difference in structure: top level containers are linked to locations records (rather than having the location be a piece of metadata in the top level container record). For digital objects, the URI is the location, but it is a piece of metadata in the digital object record, instead of a record in its own right.  

## Principles
- A digital object is used to locate digital instances of materials. 
- The primary record to describe digital material exists in the same place as that of non-digital material: resources and archival objects.
- Digital objects are used the same for born-digital, made-digital, and received-digital material. It doesn’t really matter, so long as the thing is digital. 
- Digital materials do not intrinsically have clear boundaries between one “object” and another “object”. However, for management of materials and to be able to use Aspace’s digital objects, we will need to define such boundaries. In doing so, we should aim for flexibility and a focus on the impact for users. 
