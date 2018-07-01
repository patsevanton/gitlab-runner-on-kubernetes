# gitlab-runner-on-kubernetes
Run GitLab Runner on a Kubernetes cluster

1. Add GitLab's official repository:

For Debian/Ubuntu/Mint
curl -L https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.deb.sh | sudo bash

For RHEL/CentOS/Fedora
curl -L https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.rpm.sh | sudo bash

2. Install the latest version of GitLab Runner, or skip to the next step to install a specific version:

For Debian/Ubuntu/Mint
sudo apt-get install gitlab-runner

For RHEL/CentOS/Fedora
sudo yum install gitlab-runner

3. Registering Runners as kubernetes

https://docs.gitlab.com/runner/register/index.html

