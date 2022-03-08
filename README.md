# nginx-modsec-docker
This is an nginx docker image with the modsecurity engine and the OWASP core ruleset, which aims to provide a pretty solid protection for your application. The image uses ubuntu by default, but feel free to change it to any base image that has the apt package manager. You can configure nginx in src/app.conf.
## Running
Build:
```bash
docker build -t nginx-modsec src/
```
Run: 
```bash
docker run -d -p 8000:80 --name nginx-modsec --rm nginx-modsec
```
