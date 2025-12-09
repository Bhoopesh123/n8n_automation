helm upgrade --install prod prometheus-community/kube-prometheus-stack -n metrics 

kubectl exec -n metrics -it prod-grafana-6cc855d986-vt7rc -- curl -v http://n8n.n8n.svc.cluster.local:5678/webhook/8c9a4ec2-6c5d-44db-9f54-363c5769959d
