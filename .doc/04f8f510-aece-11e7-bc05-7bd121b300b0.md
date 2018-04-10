[README](/) / [Technical](0e9eb851-aec6-11e7-9592-978508c84318.md) / [Architecture](d6d68f40-aec7-11e7-894f-6b718994da22.md) / [Servers](d6d68f41-aec7-11e7-894f-6b718994da22.md) / [Transcoding](04f8f510-aece-11e7-bc05-7bd121b300b0.md)

# Transcoding

This server hosts the following components:

- Transcoder which will be used by the system to perform media conversions

This is a Linux (Ubuntu) machine and it will hold the transcoder library (FFmpeg) required by the system to convert media files used by the applications in the Web server.

It is built through ansible's `encode` playbook which is executed in the flow of the `servers` playbook.