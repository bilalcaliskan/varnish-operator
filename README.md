# Varnish Operator

### Sample Commands
Create a project directory for your project and initialize the project:
```shell
operator-sdk init --domain docker.io --repo github.com/bilalcaliskan/varnish-operator
```

Create a simple Varnish API:
```shell
operator-sdk create api --group cache --version v1alpha1 --kind Varnish --resource --controller
```

Build and push your operator’s image:
```shell
make docker-build docker-push IMG="docker.io/bilalcaliskan/varnish-operator:v0.0.1"
```