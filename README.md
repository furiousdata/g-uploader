# Google Drive Uploader

A simple node web server that helps user to download files from web and upload to Google Drive.

## Getting Started

Simply clone the repo to your local or your host machine. You can, if you want to, use Docker to host the app instead.
Here is my docker image---> https://hub.docker.com/r/capriciousduck/g-uploader

Following is the docker command to run this app in a container.
```
docker run -d --name g-uploader \
--restart always \
-v /some/path/on/host:/g-uploader/Downloads \
-p 8080:3000 capriciousduck/g-uploader
```
### Prerequisites

- Aria2
- Node with NPM

### Installing

Simply run `npm install` inside the repo directory.

### Configuration

To control access to the server, you can configure basic settings in `config.json`.  
```
"server": {
  "username": "admin",
  "password": "google",
  "port": 3000
}
```
### Starting 

Simply run `npm start`
