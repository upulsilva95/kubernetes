# Deploy a Production Ready Kubernetes Cluster

## Initial Commands

```bash
apt-get install -y apt-transport-https ca-certificates curl

curl -fsSLo /usr/share/keyrings/kubernetes-archive-keyring.gpg https://packages.cloud.google.com/apt/doc/apt-key.gpg

echo "deb [signed-by=/usr/share/keyrings/kubernetes-archive-keyring.gpg] https://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee /etc/apt/sources.list.d/kubernetes.list

apt-get update
apt-get install -y kubectl
apt install python3-pip -y


git clone https://github.com/kubernetes-sigs/kubespray.git

cd kubespray
pip3 install -r requirements.txt

```


