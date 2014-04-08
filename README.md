Rundeck hybrid login module
===========================
Overview
--------
This login module provides the possibility for a user to be authenticated via LDAP and to be authorized (get mapped to a Rundeck role) via the *.properties file.

Prerequisites
-------------
Assuming Rundeck 2.0+ is installed.

Build
-----
Use `Ant` to build the module. The result of the build will be available under `build` directory.

Installation
------------
Stop the Rundeck server:<br/>
`rundeckd stop`<br/>
Copy the hybrid-login library (From the build directory):<br/>
`cp rundeck-hybrid-login-ext-<version>.jar $RDECK_BASE/exp/webapp/WEB-INF/lib`<br/>
Also copy jetty-all.jar (From the build direcotry): <br/>
`cp jetty-util-7.6.0.jar $RDECK_BASE/exp/webapp/WEB-INF/lib/`<br/>
Start the Rundeck server:<br/>
`rundeckd start` <br/>
