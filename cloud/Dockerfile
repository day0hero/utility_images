FROM registry.access.redhat.com/ubi8/ubi

RUN dnf install -y \
yum-utils && \
yum-config-manager --add-repo https://rpm.releases.hashicorp.com/RHEL/hashicorp.repo && \
dnf -y install \
python3 \
git \
terraform \
openssh-clients && \
dnf clean all && \
pip3 install --no-cache-dir --upgrade pip && \
pip3 install --no-cache-dir \
pip \
ansible \
openshift \
boto3 \
botocore \
awscli \
azure-cli \
pyOpenSSL \
requests \
cryptography \
passlib && \
# Install the ansible collections
ansible-galaxy collection install \
containers.podman \
kubernetes.core
