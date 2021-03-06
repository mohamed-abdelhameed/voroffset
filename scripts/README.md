### Replicability

To reproduce Figure 19 of the paper, simply run the bash script `./fig19.sh` from the terminal.
This will download the input data, compile and run the code. To produce the rendering in the paper, you will need to use [PyRenderer](https://github.com/qnzhou/PyRenderer) and Mitsuba. Those are available via docker. Make sure that [docker](https://docs.docker.com/storage/storagedriver/overlayfs-driver/) is configured with the `overlay2` driver enabled. Otherwise, you may simply open the resulting meshes from the `data/output/` folder that are produced by the script.

:warning: This script uses Docker, which might require to be run with sudo access. If you use a recent version (>= 19.3), you can add yourself to the `docker` group (root-equivalent) as documented [here](https://docs.docker.com/install/linux/docker-ce/ubuntu/):

```
sudo usermod -aG docker your-user
```
