# Helm Assessment

This projects aims to complete the following:

1. Write an nginx.conf for a simple nginx deployment that

    - Answers "Hello world from <my-ip>" on the root endpoint

    - Has a health check at /healthz that returns a 200 and {"status":"healthy"} in valid JSON

 

2. Write a helm chart to deploy nginx with that nginx.conf. Helm chart should include:

    - Deployment object that pulls a stock nginx image, configmap object to load nginx.conf into the deployment

    - Service to provide HTTP access to nginx

    - Helm values file that parameterizes the image used by the deployment

    - Extra credit, build HPA into the helm chart to react to CPU load