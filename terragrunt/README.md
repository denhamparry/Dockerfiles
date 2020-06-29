# Terragrunt

## Build

```bash
$ docker build --build-arg TERRAGRUNT=v0.23.30 -t denhamparry/terragrunt:v0.23.30 .
```

## Run

```bash
$ docker run -ti --rm -v $HOME/.aws:/root/.aws -v ${HOME}/.ssh:/root/.ssh -v `pwd`:/apps denhamparry/terragrunt bash
```

## References

- [Terragrunt](https://terragrunt.gruntwork.io/)
- [Github](https://github.com/gruntwork-io/terragrunt/)
  - [Releases](https://github.com/gruntwork-io/terragrunt/releases/)