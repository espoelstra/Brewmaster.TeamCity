###Overview
Using the latest image of Windows Server 2012 having the latest version of JDK, it will install and configure [TeamCity server](https://www.jetbrains.com/teamcity/).

###Virtual Machine (VM)
One VM will be created with a dedicated data disk for storing TeamCity data.The input parameter 'UseInternalHSQLDBEngine' determines whether to use the internal HSQLDB database or an external database. Configuring an external database has to be performed manually via the TeamCity web portal.

###Teamcity Details
1.TeamCity server is installed as a windows service running on the local system account.
2.Web Portal - `http://<TeamCityCloudService>.cloudapp.net:<TeamCityConnectionPort>`

###Limitations
The template does not setup the administrator account. As soon as the template completes execution, access the TeamCity web portal immediately to setup the administrator. On first accessing the TeamCity web portal you will prompted with a 'License Agreement' page. Upon accepting the agreement you will be taken to the page for setting up administrator.

###References
Please refer to the following links for more information on TeamCity installation and configuration.
> - [Installing and Configuring TeamCity Server](https://confluence.jetbrains.com/display/TCD8/Installing+and+Configuring+the+TeamCity+Server)
> - [Setting up External Database](https://confluence.jetbrains.com/display/TCD8/Setting+up+an+External+Database)
