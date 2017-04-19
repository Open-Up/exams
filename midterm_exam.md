# Mid-term exam

## System administration

### Description

A company wants to enable file sharing for it's employees. They identified Owncloud [https://owncloud.org/](https://owncloud.org/). They decided to hire you to do a company grade installation of this product.

### 0. Preparation

Points: 2

You will create two virtual machines from the base image. One will be named **db-server**, the second one will de named **web-server**.

Configure an additionnal network interface on them. This additionnal interface should then be configured in **bridge** mode. This would allow you to access the web sites from your computer.

*Call instructor for validation*

### 1. Setting up data base

Points: 5

On **db-server** you will need to install **mariaDB**.

You will add the opportunity for the administrator to administer it from **phpMyAdmin**.

Create a **owncloud** datbase. It should be accessible from **localhost** and **web-server**.

Create a **owncloud** user with full rights on owncloud database.

*Call instructor for validation*

### 2. Setting up the web server

Points: 4

On **web-server**, install **owncloud**. It should rely on the database **owncloud** you created on **db-server**.

*Call instructor for validation*

### 3. HTTPS

Points: 4

On **web-server** install **nginx** and use it to access **owncloud**.

You will create self-signed SSL certificate and use them to secure NGinx SSL connection. You will also force redirection from http to https.

### 4. Virtual hosting

Points: 2

**nginx** on **web-server** should also allow you to access **phpmyAdmin** installed on **db-server** in HTTPS.

*Call instructor for validation*

### 4. Additional FTP

Points: 3

Marc, from the Financial service, is using a Script for FTP synchronisation of documents. He needs FTP read access to his owncloud folder.

Create him a UNIX user. Install **proftpd** and allow Marc to have read only access to his **owncloud** folder.

*Call instructor for validation*


