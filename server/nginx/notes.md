# NGINX
https://www.aosabook.org/en/nginx.html
https://www.youtube.com/watch?v=1ndlRiaYiWQ


         request

client ---------> server

        response

       <---------


## nginx 
- an open source software
- web server for reverse proxying, caching and load balancing
- provides HTTP server capabilities
- designed for maximum performance and stability
- functions a proxy server for email (IMAP, POP3 and SMTP)
- uses a non-threaded and event-driven architecture
- event driven model, asyncronous 

### architecture

![](./diagrams/infographic-Inside-NGINX_process-model.png)

![](./diagrams/nginx-architecture.jpg)

MASTER 
 
  |
 
WORKER, WORKER, WORKER (can be more then one)


master : reading and validating configuration (in general)


cache loader 

cache Manager : cache expiration and invalidation

###### CACHING 


## why use NGINX 
- ease of installation and maintaenance
- reduces the wait time for users 
- improves performance
- load balancing 
- offers scalability
- on the fly upgrades : patch and update without having downtime

# CONFIGURATONS SETTINGS
-> the core setting of NGINX are mainly configured in the \textbf{nginx.conf}
file. The configuration file is mainly structured into Contexts

Contexts : event contexts, and http contexts 

:::
worker_processes : setting that define the number of worker_processes 
that nginx will use, usually the same as cpu cores (in general). 
nginx : single threaded 

worker_connections : maximum number of simultaneusly connections for each
worker_processes. 

access_log & error_log : logger :: for debugging or traubleshooting

gzip : compression of nginx response ::::::: need more reading 


## how to install nginx 
1. install nginx 
2. adjust firewall
3. check ur server 
4. manage the nginx process 



