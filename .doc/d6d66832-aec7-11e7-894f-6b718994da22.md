[README](/) / [Technical](0e9eb851-aec6-11e7-9592-978508c84318.md) / [Architecture](d6d68f40-aec7-11e7-894f-6b718994da22.md) / [Servers](d6d68f41-aec7-11e7-894f-6b718994da22.md) / [Web](d6d66832-aec7-11e7-894f-6b718994da22.md)

# Web

This server hosts the following components:

- Front-end management system
- Back-end core and APIs system

This is a Linux (Ubuntu) machine and it will hold the web server (NGINX) required by both applications as well as PHP and required JS modules.

It is built through ansible's `web` playbook which is executed in the flow of the `servers` playbook.

The Front-end system can be deployed at any time through the `deploy-front-end` task which is executed in the flow of the `deploy` playbook. Analogously, the Back-end core can be deployed through the `deploy-core` task executed by the same playbook.