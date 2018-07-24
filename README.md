# Jenkins CI build stack
contains:
- [Jenkins](https://jenkins.io/) (lts)
- [Docker CE](https://docs.docker.com/install/) (latest)
- [Node.js](https://nodejs.org/en/) 8.x 
- [.NET Core 2.1 SDK](https://www.microsoft.com/net/download?initial-os=linux)
- [Angular CLI](https://cli.angular.io/) (latest)

to run, just type:
```
docker run -d -p 8080:8080 \
  -v /var/run/docker.sock:/var/run/docker.sock \
  -v jenkins_home:/var/jenkins_home \
  --restart always \
  --name jenkins \
  fixerapps/jendo
```

Have a Fun ;)