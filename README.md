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



<table cellpadding='1' cellspacing='1'>
<tr>
<th style='text-align: center;'>Package</th><th style='text-align: center;'>Repo/th><th>Demo</th></tr>
<tr><td><a href='https://openexchange.intersystems.com/package/Clinical-Mindmap-Viewer'>Clinical Mindmap Viewer</a></td>
<td><a href='https://openexchange.intersystems.com/package/Clinical-Mindmap-Viewer''>excellent 6* package</a><derepo/td>
<td><a href='https://openexchange.intersystems.com/package/Clinical-Mindmap-Viewer''>excellent 6* package</a><demo/a></td>
</table>

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
