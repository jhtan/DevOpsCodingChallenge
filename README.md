# DevOps Coding Challenge

## Hello World Docker Image

### Create the image
    $ docker build -t jhtan/hello-world-html:0.1 .

### Start the image
    $ docker run -d -p 80:80 jhtan/hello-world-html:0.1

## Hello World image running with Helm

### Installing the chart
    $ helm install hello-world helloworld/ --values helloworld/values.yaml

### Forwardint the port for test
    $ kubectl port-forward hello-world-6c54fdf68d-fhd7z 8080:80

··