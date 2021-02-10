# Deploy Jenkins in Kubernetes using Helm
This repository has a `helm` chart for setting up a simple Jenkins master for running in Kubernetes.
It also contains a custom docker file to build Jenkins image with a Docker-in-Docker kind of setup. 
### Refererence: 

-   https://kubernetes.io/docs/concepts/workloads/pods/init-containers/    
-   [Docker-in-Docker for CI](https://jpetazzo.github.io/2015/09/03/do-not-use-docker-in-docker-for-ci/#:~:text=The%20primary%20purpose%20of%20Docker,into%20your%20Jenkins%20container%20instead.)


# Usage
Clone the repository and navigate to the jenkinschart folder.

```sh
$ cd jenkinschart/
```

# Deploy the Jenkins Helm Chart

Prerequisite: 
   -    [Helm](https://helm.sh/docs/intro/install/) installation on local machine.
   -    Either minikube or any other cluster configured.

   ```sh
    $ helm upgrade --install jenkins -n jenkins ./helm
   ```
   Refer [here](https://helm.sh/docs/intro/using_helm/) for Helm usage.

The folder also contains a values.yaml which you can configure as per your requirement.


## License
Apache 2.0 © [Parag Bawane]()
