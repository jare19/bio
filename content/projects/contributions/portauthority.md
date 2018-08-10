{
    "title":"Portauthority",
    "link":"https://github.com/target/portauthority",
    "image":"/img/pa.png",
    "description":"Port Authority is an API service that provides vulnerability assessments for Docker images.",
    "tags":["Go","Glide","Clair","Docker","Kubernetes","Minikube","Artifactory","Containers","Security","API","REST","Google Cloud Platform","PortAuthority","Drone.io",
            "GitHub Enterprise","CLI"],
    "weight":"13",
    "sitemap": {"priority": "0.8"},
    "featured": false
}

[![Build Status](https://travis-ci.org/target/portauthority.svg?branch=master)](https://travis-ci.org/target/portauthority/builds)

Port Authority is a solution that I helped develop at Target. I was included in the development after it was 1/2 way complete. I was able to enable scanning of images pulled from Docker Hub (exisiting functunality was to scan images from private repos), as well as create a drone.io plugin to enable pipeline scanning of a container in github enterprise. It was my first real world experience with Go and API development.  The final product is not perfect but it was a great learning experience and gets the job done.


#### From the README:
The Port Authority API is capable of orchestrating scans of individual public or private images as well as scanning entire private Docker registries like [Docker Hub](https://hub.docker.com), [Google Container Registry](https://cloud.google.com/container-registry/) or [Artifactory](https://jfrog.com/artifactory/). To accomplish this, Port Authority breaks each Docker image into layers and sends it to the open source static analysis tool [Clair](https://github.com/coreos/clair) in the backend to perform the scans and identify vulnerabilities. Upon completion of this workflow Port Authority maintains a manifest of the images and scan results.

Port Authority also supplies developers with customizable offerings to assist with the audit and governance of their container workloads. Port Authority provides a webhook that when leveraged by a [Kubernetes](https://github.com/kubernetes/kubernetes) admission controller will allow or deny deployments based off of user-defined policies and image attributes. Port Authority then achieves run-time inspection by integrating with Kubernetes to discover running containers and inventorying those deployed images for scanning.