# Docker Demo Directory
This is a list of repos to start demos based on packages   
available in IPM. It is mainly targeted at packages where   
a demo with Docker is not included in the source repo.  

It is not a clone of the original repo but uses the IPM        
package the same way you would do  in your own IRIS instance.    
Where required and appropriate also some test data are added.    
WebTerminal and PasswordLess access is always added.    

The attempt is to use only IRIS community edition.  For some   
rare cases (e.g. ECP, MIRROR) you have to  provide your own license.    
In any case, checking the installation instructions and the test  
guide of the selected repo  - if available -  is required. 

| OEX package | Repo | Demo |   
| --- | --- | --- |   
| <a href='https://openexchange.intersystems.com/package/BulkProfile-HL7RoutingRules'>BulkProfile_HL7RoutingRules</a> | <a href='https://github.com/alexatwoodhead/BulkProfile_HL7RoutingRules'>repo</a> | <a href='https://github.com/rcemper/DD_BulkProfile_HL7RoutingRules'>demo</a> | 631
| <a href='https://openexchange.intersystems.com/package/iknow-utils'> iknow-utils </a> | <a href='https://github.com/bdeboe/isc-iknow-utils'>repo</a> | <a href='https://github.com/rcemper/DD_isc-iknow-utils'>demo</a> | 723
| <a href='https://openexchange.intersystems.com/package/Ikon'>Ikon</a> | <a href='https://github.com/AndreiLN/Ikon'>repo</a> | <a href='https://github.com/rcemper/DD_Ikon'>demo</a> | 294
| <a href='https://openexchange.intersystems.com/package/iris-mail'>iris-mail</a> | <a href='https://github.com/rcemper/pr_iris-mail'>repo</a> | <a href='https://github.com/rcemper/DD_iris-mail'>demo</a> | 613
| <a href='https://openexchange.intersystems.com/package/isc-json'>isc-json</a> | <a href='https://github.com/intersystems/isc-json'>repo</a> | <a href='https://github.com/rcemper/DD_isc-json'>demo</a> | 622
| <a href='https://openexchange.intersystems.com/package/MDX-Query-Auditing-Samples'>MDX Query Auditing Samples</a> | <a href='https://github.com/sduncan01/CubeAuditing'>repo</a> | <a href='https://github.com/rcemper/DD_CubeAuditing'>demo</a> | 83
| <a href='https://openexchange.intersystems.com/package/MDX2JSON'>MDX2JSON</a> | <a href='https://github.com/intersystems-ru/Cache-MDX2JSON'>repo</a> | <a href='https://github.com/rcemper/DD_mdx2json'>demo</a> | 47
| <a href='https://openexchange.intersystems.com/package/Message-Bank'>Message Bank</a> | <a href='https://github.com/rcemper/DK_messagebank'>repo</a> | <a href='https://github.com/rcemper/DK_messagebank'>demo</a> | 212
| Total **8** | 2024-02-25|22:39:22 |

 
### Prerequisites
Make sure you have [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and [Docker desktop](https://www.docker.com/products/docker-desktop) installed.
### Installation
Clone/git pull the repo into any local directory
```
$ git clone https://github.com/****************.git
```
To build and start the container run:
```
$ docker compose up -d && docker compose logs -f
```
### Generic Testing   
Open IRIS console     
```
$ docker-compose exec iris iris session iris
USER>
```
or use **WebTerminal**
```
http://localhost:42773/terminal/
```
To access IRIS System Management Portal
```
http://localhost:42773/csp/sys/UtilHome.csp
```
