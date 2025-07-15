# cdevops-gitea
k8s gitea lab to take dev (sqlite based) to prod (mysql based)

TLDR;

```bash
pip install ansible kubernetes
ansible-playbook up.yaml
kubectl port-forward svc/gitea-http 3000:3000
```

Now you should be able to access gitea in development mode.

The challenge is to run this in production mode from a prod folder at the same level as the dev folder with it's own up, down and values.yaml.

### Points to Cover

## Marking

|Item|Out Of|
|--|--:|
|use [the gitea helm](https://gitea.com/gitea/helm-gitea) to make the repository data persistent|4|
|make gitea use external database|4|
|Use [this article](https://blog.techiescamp.com/using-ngrok-with-kubernetes/) to expose your gitea instance publically|2|
|||
|total|10|
