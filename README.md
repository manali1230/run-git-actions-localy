# Run git-actions Locally

1. Install Docker on your respective operating system.

[Install-Docker-on-Mac](https://docs.docker.com/desktop/install/mac-install/)<br>
[Install-Docker-on-Ubuntu](./install-docker.sh)<br>


2. Install nektos/act

```
curl -s https://raw.githubusercontent.com/nektos/act/master/install.sh | sudo bash
```

For more details [check](https://github.com/nektos/act.git) nektos/act repository

3. Run your workflow by using below command - 

```
./bin/act -W .github/workflows/main.yaml -P test=catthehacker/ubuntu:act-18.04
```

Where, \
`-W` - used to pass your workflow file \
`-P` - used to pass runner docker image

