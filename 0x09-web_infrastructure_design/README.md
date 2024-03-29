#  0x09-web_infrastructure_design.

At the end of this project you are expected to be able to explain, without the help of Google:

> You must be able to draw a diagram covering the web stack you built with the sysadmin/devops track projects

You must be able to explain what each component is doing

You must be able to explain system redundancy

Know all the mentioned acronyms: LAMP, SPOF, QPS

# File Descriptions

Each file contains a link to an image hosted on Imgur. These images are based on the following requirements:

    0-simple_web_stack

On a whiteboard, design a one server web infrastructure that hosts the website that is reachable via www.foobar.com. Start your explanation by having a user wanting 

to access your website.

You must use:

1 physical server

1 web server (Nginx)

1 application server

1 application files (your code base)

1 database (MySQL)

1 domain name foobar.com configured with a www record that points to your server IP 8.8.8.8

![WID](https://user-images.githubusercontent.com/99593138/191125507-19088d04-7d94-4095-9e1f-5b9c4c769bb4.jpg)

     1-distributed_web_infrastructure

On a whiteboard, design a three servers web infrastructure that host the website www.foobar.com.

You must add to 0-simple_web_stack:

 2 physical servers

1 web server (Nginx)

1 application server

1 load-balancer (HAproxy)

1 application files (your code base)

1 database (MySQL)

![WID1](https://user-images.githubusercontent.com/99593138/191125994-6563ed42-7e8d-4e6a-9cba-799f298d3c07.jpg)


    2-secured_and_monitored_web_infrastructure

On a whiteboard, design a three servers web infrastructure that host the website www.foobar.com, it must be secured, serve encrypted traffic and be monitored.

You must add to 1-distributed_web_infrastructure:

3 firewalls

1 SSL certificate to serve www.foobar.com over HTTPS

3 monitoring clients (data collector for Sumologic or other monitoring services)

![WID3](https://user-images.githubusercontent.com/99593138/191126029-9ac4e2a8-0fa1-4080-8698-f290e197edbc.jpg)


     3-scale_up

You must add to 2-secured_and_monitored_web_infrastructure:

1 physical server

1 load-balancer (HAproxy) configured as cluster with the other one

Split components (web server, application server, database) with their own server.

![WID3](https://user-images.githubusercontent.com/99593138/191126064-579ff049-7275-4919-9a76-5e9735064c9e.jpg)


