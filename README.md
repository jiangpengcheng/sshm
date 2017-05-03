# sshm
A simple SSH bookmarks script that help remember the history of ssh command.

# Install
Just put sshm and sshm-update into `/usr/local/bin` or somewhere else.

Run commands below to init:

```shell
mkdir ~/.sshm
touch ~/.sshm/.data
```

And add the follow lines to ~/.bashrc or any other shell's rc file:
```shell
ssh() {
  /usr/bin/ssh "$@" && sshm-update "$*"
}
```

Source the rc file or logout/login to make these lines activated.

That's all.

# Usage
Run `sshm` and it will show you enough help messages.
