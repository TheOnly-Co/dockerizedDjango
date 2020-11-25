# dockerizedDjango

[![CircleCI](https://circleci.com/gh/TheOnly-Co/dockerizedDjango.svg?style=svg)](https://circleci.com/gh/TheOnly-Co/dockerizedDjango)

## How to

1. Run server

   - make sure you have python3 and pip installed on your machine
   - `cd myDjango`
   - run `python3 manage.py runserver`
   - go to [localhost:8000/hello](http://localhost:8000/hello) in the browser to see the information

2. Docker Image + Kubernetes

   - run `docker pull 0857/mydjango_web:latest`
   - run `kubectl create -f deployment.yaml` in Kubernetes nodes
   - run `kubectl port-forward svc/mydjango-web-svc 8000`
   - go to [localhost:8000/hello](http://localhost:8000/hello) in the browser to see the information
