[README](/) / [Technical](0e9eb851-aec6-11e7-9592-978508c84318.md) / [Architecture](d6d68f40-aec7-11e7-894f-6b718994da22.md) /

# Architecture

Tuningfork Médiathèque will be a multitiered system comprised roughly of the following sub-applications or modules:

* A front-end system to allow the administrative users of Tuningfork to perform the actions required to fulfill the processes related to media creation/translation/review/publication
* A back-end system to provide the APIs necessary in order to manage and serve the media files as well the data and schema to control the process and interactions themselves. These APIs will be consumed both by the front-end system mentioned as well as Tuningfork applications that handle media
* A DB schema to support the management processes and media handling mentioned
* A transcoding system to perform media transcoding for the files managed by the Médiathèque as necessary

![Architecture*](./Architecture.png)

The infrastructure envisioned to support these will be deployed through the ansible pipelines in this repository.

Please follow the below link to view the breakdown of the servers involved.

---

# Summary

* [Servers](d6d68f41-aec7-11e7-894f-6b718994da22.md)
