# eyewitness-docker
An EyeWitness Docker Container leveraging Ubuntu

Objective: To have a docker container encapsulating EyeWitness for easy portability and usage.

## Reference(s):
  https://github.com/ChrisTruncer/EyeWitness  --> 
  https://github.com/FortyNorthSecurity/EyeWitness
  
  https://www.christophertruncer.com/eyewitness-2-0-release-and-user-guide/
  
  https://hub.docker.com/r/whiteoaksecurity/docker-eyewitness/~/dockerfile/

---

`docker build --tag eyewitness .`

Also available pre-built from docker hub
`docker pull ly4e/eyewitness-docker`


## Usage Example(s):
```
docker container run --rm -it -v $(pwd)/EyeWitness:/tmp/EyeWitness/ [docker_image_name] --headless --single http://www.google.com

docker container run --rm -it -v $(pwd)/EyeWitness:/tmp/EyeWitness/ [docker_image_name] --headless -f /tmp/EyeWitness/file_of_urls.txt
```

### Version history:
version: 0.1.0 historical original image years old

version: 1.0.0 updated image similar build process