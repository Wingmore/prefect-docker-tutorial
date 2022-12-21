# prefect-docker-tutorial
Prefect docker tutorial

Somehow there is a Client error ‘404 Not Found’ when trying to deploy a flow


Steps to reproduce:

```
git clone https://github.com/Wingmore/prefect-docker-tutorial.git

cd prefect-docker-tutorial

prefect deployment build ./log_flow.py:log_flow -n log-flow-docker-tutorial -ib docker-container/log-tutorial -q test -o log-flow-docker-deployment.yaml -a

prefect deployment run log-flow/log-flow-docker-tutorial 
```

