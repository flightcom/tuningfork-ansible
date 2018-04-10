[README](/) / [Technical](0e9eb851-aec6-11e7-9592-978508c84318.md) / [Architecture](d6d68f40-aec7-11e7-894f-6b718994da22.md) / [Servers](d6d68f41-aec7-11e7-894f-6b718994da22.md) / [Db](ec37d460-aecd-11e7-b4e2-fb7a6b2429a0.md)


# DB

This server hosts the following components:

- DB schema to support the management processes and media handling 

This is a Linux (Ubuntu) machine and it will hold the DBMS (MariaDB) required by the system which will be accessible by the applications in the Web server through the CDDMD network.

It is built through ansible's `db` playbook which is executed in the flow of the `servers` playbook.