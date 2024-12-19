# Prometheus, Grafana implementation

## Prequisite 
Please ensure all the tools required are installed\
1. Docker desktop
2. Minikube
3. Kubernetes

## Prometheus, Grafana
1. Install Chocolatey
https://chocolatey.org/install

2. Install Helm
Use this command to install helm `choco install kubernetes-helm`

3. Port forward Prometheus
`kubectl port-forward service\{prometheus-server} 9090:9090`

4. Port forward Grafana
`kubectl port-forward service\{grafana} 3100:8080`

## Application
1. Build the application Docker image
2. Create the application deployment and service yaml for kubernetes
3. Load the application Docker image to Minikube
4. Create K8s pod for the application


## References
https://gitlab.com/nanuchi/youtube-tutorial-series/-/blob/master/prometheus-exporter/install-prometheus-commands.md \
https://www.youtube.com/watch?v=QoDqxm7ybLc \
https://www.youtube.com/watch?v=mLPg49b33sA
