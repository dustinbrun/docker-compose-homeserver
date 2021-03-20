# docker-compose-homeserver
Docker Compose application templates for homeserver setup

In this repository I share my docker-compose files, which I use in my homeserver environment.

<br>

# How to use these Files
These Containers are designed to work on a Debain based machine.
<br>You need to install docker (see https://docs.docker.com/engine/install/debian/) 
<br>and docker-compose (see https://docs.docker.com/compose/install/). 
<br>I also recommend to install portainer to monitor your created containers (see https://documentation.portainer.io/v2.0/deploy/ceinstalldocker/)

For each application there is a seperate folder.
You need to place these folders in your home-directory, for example into `/root`. The docker-compose files are designed in a way, that all configuration- and data-folders are stored in these application folders. If you want to backup your containers you simply backup these folders and you can restore them easily.

To deploy a container, go into the application-folder and type: 
```
docker-compose up -d
``` 


# Application List
| Name      | Description  |
| --------  | ------------ |
| gitea     | self-hosted Git service |
| hedgedoc  | collaborative (multi user) markdown editor |
| icecast   | audio streaming server |
| nextcloud | online file server / personal cloud |
| onlyoffice | webbrowser based office software, used with nextcloud 
| npm       | nginx proxy manager, nginy proxy with web ui |
| wordpress | content management system (CMS) / blog software |
| synapse   | Matrix server, personal chat server |
| matrix-extensions | synapse-admin - User management for synapse with web ui |
|                   | element-web - Web Messenger client for matrix/element |
| duplicati | Automated backup software with web ui |
| overleaf | web based latex text editor with live preview (sharelatex) |
| lychee | web photo gallery |
| piwigo | web photo gallery <- Best one in my Opinion |
| picapport | web photo gallery |
| Grafana | Graphical Interface for databases |
| Influxdb | time series database server |

<br><br>
# Sources
Most of these Files I have not written myself. I found these accross the web and somtimes adapted them to my needs. 

Mainly these are the template files created by the respective developer of the application. 

dustinbrun