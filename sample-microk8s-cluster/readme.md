### perequisit : VMs with ubuntu 18+ (preferably under same subnet, minimum 2Vcpu and 2GB memory, allow port 22)
- login to master node run following script, follow instructions
```
sudo git clone https://github.com/DhamodharReddy/team-repo && cd team-repo/sample-microk8s-cluster && sudo ./master.sh
```
- login to workernodes and run following script, follow instructions
```
sudo git clone https://github.com/DhamodharReddy/team-repo && cd team-repo/sample-microk8s-cluster && sudo ./worker.sh
```
- verify your cluster, run following script on master
```
microk8s kubectl get nodes
```
