## **Prerequisites :**
- Two ubuntu servers 

## **Setup k3s cluster**
<p> Install k3s using below command on 1st vm </p>

```
curl -sfL https://get.k3s.io | INSTALL_K3S_VERSION=v1.20.7+k3s1 sh -
```

<p> Copy the accesskey token from below command </p>

```
cat /var/lib/rancher/k3s/server/node-token
```
<p>Login to another VM manually and excute below command & paste the server IP and accesskey </p>

```
curl -sfL https://get.k3s.io | INSTALL_K3S_VERSION=v1.20.7+k3s1 K3S_URL=https://<Server-IP>:6443 K3S_TOKEN=<Access-key> sh -
```
<p> Paste this command in master node to get nodes </P>

```
sudo k3s kubectl get nodes
```
