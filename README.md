# Deploy Jenkins in Kubernetes using Helm
This repository has a `helm` chart for setting up a simple Jenkins master for running in Kubernetes.

# Deploy the Jenkins helm chart
# (same command for install and upgrade)
<TODO>
```

### Data persistence
By default, in Kubernetes, the Jenkins deployment uses a persistent volume claim that is mounted to `/var/jenkins_home`.
This assures your data is saved across crashes, restarts and upgrades.