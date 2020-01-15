# Install docker offline
## Install static binaries

Download the static binary archive. Go to https://download.docker.com/linux/static/stable/ (or change stable to nightly or test), choose your hardware platform, and download the .tgz file relating to the version of Docker Engine - Community you want to install.

Extract the archive using the tar utility. The dockerd and docker binaries are extracted.
```
$ tar xzvf /path/to/<FILE>.tar.gz
```
Optional: Move the binaries to a directory on your executable path, such as /usr/bin/. If you skip this step, you must provide the path to the executable when you invoke docker or dockerd commands.
```
$ sudo cp docker/* /usr/bin/
```
Start the Docker daemon:
```
$ sudo dockerd &
```
If you need to start the daemon with additional options, modify the above command accordingly or create and edit the file /etc/docker/daemon.json to add the custom configuration options.
