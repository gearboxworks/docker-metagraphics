![Gearbox](https://gearboxworks.github.io/assets/images/gearbox-logo.png)


# metagraphics Docker container service for [Gearbox](https://github.com/gearboxworks/)
This is the repository for the [metagraphics]() Docker container implemented for [Gearbox](https://github.com/gearboxworks/).


## Repository Info
GitHub commit: ![commit-date](https://img.shields.io/github/last-commit/gearboxworks/docker-metagraphics?style=flat-square)

GitHub release(latest): ![last-release-date](https://img.shields.io/github/release-date/gearboxworks/docker-metagraphics) ![last-release-date](https://img.shields.io/github/v/tag/gearboxworks/docker-metagraphics?sort=semver) [![release-state](https://github.com/gearboxworks/docker-metagraphics/workflows/release/badge.svg?event=release)](https://github.com/gearboxworks/docker-metagraphics/actions?query=workflow%3Arelease)


## Supported versions and respective Dockerfiles
| Service | GitHub Version | Docker Version | Docker Size | Docker Tags |
| ------- | -------------- | -------------- | ----------- | ----------- |
| metagraphics | ![metagraphics](https://img.shields.io/badge/metagraphics-1.0.0-green.svg) | [![Docker Version)](https://img.shields.io/docker/v/gearboxworks/metagraphics/1.0.0)](https://hub.docker.com/repository/docker/gearboxworks/metagraphics) | [![Docker Size](https://img.shields.io/docker/image-size/gearboxworks/metagraphics/1.0.0)](https://hub.docker.com/repository/docker/gearboxworks/metagraphics) | _([`1.0.0`, `1.0`, `latest`](https://github.com/gearboxworks/docker-metagraphics/blob/master/versions/1.0.0/DockerfileRuntime))_ |


## About this container.
A driving force behind [Gearbox](https://github.com/gearboxworks/) is to improve the user experience using software, and especially for software developers.

Our vision is to empower developers and other software users to quickly and easily use almost any version of a software service, command line tool or API without without first getting bogged down with installation and configuration.

In other words, our vision for [Gearbox](https://github.com/gearboxworks/) users is that software "**just works**".


## Using this container.
This container has been designed to work within the [Gearbox](https://github.com/gearboxworks/) framework.
However, due to the flexability of Gearbox, it can be used outside of this framework.

There are three methods:

## Method 1: Using launch
`launch` is a tool specifically designed to interact with a Gearbox Docker container.

It provides three important functional areas, without any Docker container learning curve:
- Allows control over Gearbox Docker containers: stop, start, create, remove.
- Build, update, modify and release Docker images.
- Acts as a proxy for interactive commands within a Gearbox Docker container.

It also provides a functional SSH daemon for connecting remotely as well as a standard set of common tools and utilities.

Further `launch` documentation can be [found here](https://github.com/gearboxworks/docker-template/blob/master/LAUNCH.md).

### Download launch
`launch` is currently in beta testing and is included along with all Gearbox Docker repos.
Once out of beta, it will be included within the Gearbox installation package.

For now, simply download the standalone `launch` binary for your O/S.
- [Mac OSX 64bit](https://github.com/gearboxworks/docker-template/raw/master/bin/Darwin/launch)
- [Linux 64bit](https://github.com/gearboxworks/docker-template/raw/master/bin/Linux/launch)
- [Windows 64bit](https://github.com/gearboxworks/docker-template/raw/master/bin/Windows/launch)


### Running launch
There are many ways to call launch, either directly or indirectly.
Additionally, all host environment variables will be imported into the container seamlessly.
This allows a devloper to try multiple versions of software as though they were installed locally.

If a container is missing, it will be downloaded and created. Multiple versions can co-exist.

Install, create, and start the metagraphics Gearbox container.

`./launch install metagraphics`

Create, and start the metagraphics Gearbox container. Run a shell.

`./launch shell metagraphics`

Create, and start the metagraphics Gearbox container with version 1.0.0 and run a shell.

`./launch shell metagraphics:1.0.0`

`./launch shell metagraphics:1.0.0 ls -l`

`./launch shell metagraphics:1.0.0 ps -eaf`


### Available commands
If metagraphics is symlinked to `launch`, then the Gearbox container will be determined automatically and the default command will be run.
All available commands for a Gearbox container will be automatically symlinked upon installation.

`./metagraphics`

Running metagraphics Gearbox container default command. If a container has a default interactive command, arguments can be supplied without specifying that command.

`./metagraphics -flag1 -flag2 variable`

`./launch metagraphics:1.0.0 -flag1 -flag2 variable`

Gearbox containers may have multiple executables that can be run. The metagraphics Gearbox container has the following available commands:
- `Magick++-config` - will execute `/usr/bin/Magick++-config` within the container.
- `MagickCore-config` - will execute `/usr/bin/MagickCore-config` within the container.
- `MagickWand-config` - will execute `/usr/bin/MagickWand-config` within the container.
- `acyclic` - will execute `/usr/bin/acyclic` within the container.
- `animate` - will execute `/usr/bin/animate` within the container.
- `annotate` - will execute `/usr/bin/annotate` within the container.
- `bcomps` - will execute `/usr/bin/bcomps` within the container.
- `ccomps` - will execute `/usr/bin/ccomps` within the container.
- `circo` - will execute `/usr/bin/circo` within the container.
- `cjpeg` - will execute `/usr/bin/cjpeg` within the container.
- `cluster` - will execute `/usr/bin/cluster` within the container.
- `compare` - will execute `/usr/bin/compare` within the container.
- `composite` - will execute `/usr/bin/composite` within the container.
- `conjure` - will execute `/usr/bin/conjure` within the container.
- `convert` - will execute `/usr/bin/convert` within the container.
- `corepdf` - will execute `/usr/bin/corepdf` within the container.
- `cwebp` - will execute `/usr/bin/cwebp` within the container.
- The default command will execute `/usr/bin/magick` within the container.
- `diff-pdf` - will execute `/usr/bin/diff-pdf` within the container.
- `dijkstra` - will execute `/usr/bin/dijkstra` within the container.
- `display` - will execute `/usr/bin/display` within the container.
- `djpeg` - will execute `/usr/bin/djpeg` within the container.
- `dot` - will execute `/usr/bin/dot` within the container.
- `dot2gxl` - will execute `/usr/bin/dot2gxl` within the container.
- `dot_builtins` - will execute `/usr/bin/dot_builtins` within the container.
- `dotty` - will execute `/usr/bin/dotty` within the container.
- `dwebp` - will execute `/usr/bin/dwebp` within the container.
- `edgepaint` - will execute `/usr/bin/edgepaint` within the container.
- `exiftool` - will execute `/usr/bin/exiftool` within the container.
- `exiftran` - will execute `/usr/bin/exiftran` within the container.
- `fax2ps` - will execute `/usr/bin/fax2ps` within the container.
- `fax2tiff` - will execute `/usr/bin/fax2tiff` within the container.
- `fdp` - will execute `/usr/bin/fdp` within the container.
- `fix-qdf` - will execute `/usr/bin/fix-qdf` within the container.
- `gc` - will execute `/usr/bin/gc` within the container.
- `gd2copypal` - will execute `/usr/bin/gd2copypal` within the container.
- `gd2togif` - will execute `/usr/bin/gd2togif` within the container.
- `gd2topng` - will execute `/usr/bin/gd2topng` within the container.
- `gdcmpgif` - will execute `/usr/bin/gdcmpgif` within the container.
- `gdparttopng` - will execute `/usr/bin/gdparttopng` within the container.
- `gdtopng` - will execute `/usr/bin/gdtopng` within the container.
- `gif2rgb` - will execute `/usr/bin/gif2rgb` within the container.
- `gif2webp` - will execute `/usr/bin/gif2webp` within the container.
- `gifbuild` - will execute `/usr/bin/gifbuild` within the container.
- `gifclrmp` - will execute `/usr/bin/gifclrmp` within the container.
- `gifdiff` - will execute `/usr/bin/gifdiff` within the container.
- `giffix` - will execute `/usr/bin/giffix` within the container.
- `gifsicle` - will execute `/usr/bin/gifsicle` within the container.
- `giftext` - will execute `/usr/bin/giftext` within the container.
- `giftogd2` - will execute `/usr/bin/giftogd2` within the container.
- `giftool` - will execute `/usr/bin/giftool` within the container.
- `gifview` - will execute `/usr/bin/gifview` within the container.
- `gm` - will execute `/usr/bin/gm` within the container.
- `gml2gv` - will execute `/usr/bin/gml2gv` within the container.
- `gnuplot` - will execute `/usr/bin/gnuplot` within the container.
- `graphml2gv` - will execute `/usr/bin/graphml2gv` within the container.
- `gv2gml` - will execute `/usr/bin/gv2gml` within the container.
- `gv2gxl` - will execute `/usr/bin/gv2gxl` within the container.
- `gvcolor` - will execute `/usr/bin/gvcolor` within the container.
- `gvgen` - will execute `/usr/bin/gvgen` within the container.
- `gvmap` - will execute `/usr/bin/gvmap` within the container.
- `gvmap.sh` - will execute `/usr/bin/gvmap.sh` within the container.
- `gvpack` - will execute `/usr/bin/gvpack` within the container.
- `gvpr` - will execute `/usr/bin/gvpr` within the container.
- `gxl2dot` - will execute `/usr/bin/gxl2dot` within the container.
- `gxl2gv` - will execute `/usr/bin/gxl2gv` within the container.
- `identify` - will execute `/usr/bin/identify` within the container.
- `img2webp` - will execute `/usr/bin/img2webp` within the container.
- `import` - will execute `/usr/bin/import` within the container.
- `jpegoptim` - will execute `/usr/bin/jpegoptim` within the container.
- `jpegtran` - will execute `/usr/bin/jpegtran` within the container.
- `lefty` - will execute `/usr/bin/lefty` within the container.
- `lneato` - will execute `/usr/bin/lneato` within the container.
- `magick` - will execute `/usr/bin/magick` within the container.
- `magick-script` - will execute `/usr/bin/magick-script` within the container.
- `mm2gv` - will execute `/usr/bin/mm2gv` within the container.
- `mogrify` - will execute `/usr/bin/mogrify` within the container.
- `montage` - will execute `/usr/bin/montage` within the container.
- `muraster` - will execute `/usr/bin/muraster` within the container.
- `mutool` - will execute `/usr/bin/mutool` within the container.
- `neato` - will execute `/usr/bin/neato` within the container.
- `nop` - will execute `/usr/bin/nop` within the container.
- `opj_compress` - will execute `/usr/bin/opj_compress` within the container.
- `opj_decompress` - will execute `/usr/bin/opj_decompress` within the container.
- `opj_dump` - will execute `/usr/bin/opj_dump` within the container.
- `optipng` - will execute `/usr/bin/optipng` within the container.
- `osage` - will execute `/usr/bin/osage` within the container.
- `pal2rgb` - will execute `/usr/bin/pal2rgb` within the container.
- `patchwork` - will execute `/usr/bin/patchwork` within the container.
- `pdfgrep` - will execute `/usr/bin/pdfgrep` within the container.
- `png-fix-itxt` - will execute `/usr/bin/png-fix-itxt` within the container.
- `pngcrush` - will execute `/usr/bin/pngcrush` within the container.
- `pngfix` - will execute `/usr/bin/pngfix` within the container.
- `pngquant` - will execute `/usr/bin/pngquant` within the container.
- `pngtogd` - will execute `/usr/bin/pngtogd` within the container.
- `pngtogd2` - will execute `/usr/bin/pngtogd2` within the container.
- `ppm2tiff` - will execute `/usr/bin/ppm2tiff` within the container.
- `prune` - will execute `/usr/bin/prune` within the container.
- `qpdf` - will execute `/usr/bin/qpdf` within the container.
- `raw2tiff` - will execute `/usr/bin/raw2tiff` within the container.
- `rdjpgcom` - will execute `/usr/bin/rdjpgcom` within the container.
- `sccmap` - will execute `/usr/bin/sccmap` within the container.
- `sfdp` - will execute `/usr/bin/sfdp` within the container.
- `stream` - will execute `/usr/bin/stream` within the container.
- `tiff2bw` - will execute `/usr/bin/tiff2bw` within the container.
- `tiff2pdf` - will execute `/usr/bin/tiff2pdf` within the container.
- `tiff2ps` - will execute `/usr/bin/tiff2ps` within the container.
- `tiff2rgba` - will execute `/usr/bin/tiff2rgba` within the container.
- `tiffcmp` - will execute `/usr/bin/tiffcmp` within the container.
- `tiffcp` - will execute `/usr/bin/tiffcp` within the container.
- `tiffcrop` - will execute `/usr/bin/tiffcrop` within the container.
- `tiffdither` - will execute `/usr/bin/tiffdither` within the container.
- `tiffdump` - will execute `/usr/bin/tiffdump` within the container.
- `tiffinfo` - will execute `/usr/bin/tiffinfo` within the container.
- `tiffmedian` - will execute `/usr/bin/tiffmedian` within the container.
- `tiffset` - will execute `/usr/bin/tiffset` within the container.
- `tiffsplit` - will execute `/usr/bin/tiffsplit` within the container.
- `tjbench` - will execute `/usr/bin/tjbench` within the container.
- `tred` - will execute `/usr/bin/tred` within the container.
- `twopi` - will execute `/usr/bin/twopi` within the container.
- `unflatten` - will execute `/usr/bin/unflatten` within the container.
- `vimdot` - will execute `/usr/bin/vimdot` within the container.
- `webpinfo` - will execute `/usr/bin/webpinfo` within the container.
- `webpmux` - will execute `/usr/bin/webpmux` within the container.
- `webpng` - will execute `/usr/bin/webpng` within the container.
- `wrjpgcom` - will execute `/usr/bin/wrjpgcom` within the container.
- `xpdf` - will execute `/usr/bin/xpdf` within the container.
- `zlib-flate` - will execute `/usr/bin/zlib-flate` within the container.


### Remote connection
ssh - All [Gearbox](https://github.com/gearboxworks/) containers have a running SSH daemon. So you can connect remotely.
To show what ports are exported to the host, use the following command.

`./launch list metagraphics`


## Method 2: GitHub repo

### Setup from GitHub repo
Simply clone this repository to your local machine

`git clone https://github.com/gearboxworks/docker-metagraphics.git`

### Building from GitHub repo
`make build` - Build Docker images. Build all versions from the base directory or specific versions from each directory.

`make list` - List already built Docker images. List all versions from the base directory or specific versions from each directory.

`make clean` - Remove already built Docker images. Remove all versions from the base directory or specific versions from each directory.

`make push` - Push already built Docker images to Docker Hub, (only for Gearbox admins). Push all versions from the base directory or specific versions from each directory.

### Runtime from GitHub repo
You can either build your container as above, or use it from DockerHub with these commands:

`make start` - Spin up a Docker container with the correct runtime configs.

`make stop` - Stop a Docker container.

`make run` - Run a Docker container in the foreground, (all STDOUT and STDERR will go to console). The Container be removed on termination.

`make shell` - Run a shell, (/bin/bash), within a Docker container.

`make rm` - Remove the Docker container.

`make test` - Will issue a `stop`, `rm`, `clean`, `build`, `create` and `start` on a Docker container.


## Method 3: Docker Hub

### Setup from Docker Hub
A simple `docker pull gearbox/metagraphics` will pull down the latest version.

### Starting
start - Spin up a Docker container with the correct runtime configs.

`docker run -d --name metagraphics-latest --restart unless-stopped --network gearboxnet gearbox/metagraphics:latest`

### Stopping
stop - Stop a Docker container.

`docker stop metagraphics-latest`

### Remove container
rm - Remove the Docker container.

`docker container rm metagraphics-latest`

### Run in foreground
run - Run a Docker container in the foreground, (all STDOUT and STDERR will go to console). The Container be removed on termination.

`docker run --rm --name metagraphics-latest --network gearboxnet gearbox/metagraphics:latest`

### Run a shell
shell - Run a shell, (/bin/bash), within a Docker container.

`docker run --rm --name metagraphics-latest -i -t --network gearboxnet gearbox/metagraphics:latest /bin/bash`

### SSH
ssh - All [Gearbox](https://github.com/gearboxworks/) containers have a running SSH daemon. So you can connect remotely.

Either use `launch` above or discover the port and SSH directly.


```
SSH_PORT="$(docker port metagraphics-latest 22/tcp | sed 's/0.0.0.0://')"
ssh -p ${SSH_PORT} -o StrictHostKeyChecking=no gearbox@localhost
```

