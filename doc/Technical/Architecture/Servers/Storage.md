[README](/) / [Technical](0e9eb851-aec6-11e7-9592-978508c84318.md) / [Architecture](d6d68f40-aec7-11e7-894f-6b718994da22.md) / [Servers](d6d68f41-aec7-11e7-894f-6b718994da22.md) / [Storage](f9484040-aecd-11e7-ad91-67e0b4f81c02.md)

# Storage

This server hosts the following components:

- The filesystem which will be used for the storage/serving of media files by the applications

This is a Linux (Ubuntu) machine and it will hold an FTP server (vsftpd) required by the system to hold/serve the files which will be accessible by the applications in the Web server through the CDDMD network.

It is built through ansible's `storage` playbook which is executed in the flow of the `servers` playbook.