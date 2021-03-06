# gitlab-runner-on-kubernetes
Run GitLab Runner on a Kubernetes cluster

1. Add GitLab's official repository:

For Debian/Ubuntu/Mint
```sh
curl -L https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.deb.sh | sudo bash
```
For RHEL/CentOS/Fedora
```sh
curl -L https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.rpm.sh | sudo bash
```

2. Install the latest version of GitLab Runner, or skip to the next step to install a specific version:

For Debian/Ubuntu/Mint
```sh
sudo apt-get install gitlab-runner
```

For RHEL/CentOS/Fedora
```sh
sudo yum install gitlab-runner
```
3. Registering Runners as kubernetes

https://docs.gitlab.com/runner/register/index.html

4. Create namespace, configmap, deployment
```sh
kubectl create -f namespace-gitlab.yaml
kubectl create -f configmap.yaml
kubectl create -f deployment.yaml
```
