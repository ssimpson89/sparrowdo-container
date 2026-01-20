# sparrowdo-container

To run, cd into your folder that contains the task shell script and `main.raku`:

```bash
podman run --rm -v $HOME/.ssh:/root/.ssh -v $(pwd):/app ghcr.io/ssimpson89/sparrowdo:latest sparrowdo --ssh_user rocky --no_sudo --sparrowfile main.raku --color --host <ip address>
```

You can also create an alias:

```bash
alias sparrowdo="podman run --rm -v $HOME/.ssh:/root/.ssh -v $(pwd):/app localhost/sparrow:dev sparrowdo"
```

And then:

```bash
sparrowdo --ssh_user rocky --no_sudo --sparrowfile main.raku --color --host <ip address>
```

For more information, please take a look at the upstream repository:

<https://github.com/melezhik/sparrowdo>
