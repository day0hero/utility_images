FROM registry.access.redhat.com/ubi8/ubi

RUN dnf install -y python3 git openssh-clients && \
dnf clean all && \
pip3 install --no-cache-dir --upgrade pip && \
pip3 install --no-cache-dir \
pip \
ansible \
openshift \
pyOpenSSL \
requests \
cryptography \
passlib && \
# Install the ansible collections
ansible-galaxy collection install \
containers.podman \
kubernetes.core
