# Network Automation Project:

## Aim:
- To implement a simple web service for the content in [index.php](index.php).

- Provision the Nginx on the web-servers and HAproxy to load-balance between servers.

## The logical network/service map:

```
(Internet)---> HAProxy	
		+--->A	|--
		+--->B	| |---> (Internal Private Network (10.0.1.0/27)	
		+--->C	|--
(Internet) --->	Bastion
```

## Provisioning of Nginx web-servers:

- Provision the Nginx servers on the webserver hosts with php packages.
- Configure the Nginx servers and restart the servers.

## Provisioning of HAproxy load-balancer: 

- Provision the  HAproxy on the load-balancer hosts.
- Configure the HAproxy and restart HAproxy servers.

