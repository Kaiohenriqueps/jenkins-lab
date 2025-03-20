# jenkins-lab
My first Jenkins lab.

## Guide to run Jenkins
Just follow the steps right [here](https://www.jenkins.io/doc/book/installing/docker/).

## Running locally
```
$ docker build -t jenkins-image .
$ docker run -d --name jenkins-container -p 8080:8080 -v ${PWD}/scripts:/scripts jenkins-image:latest
```