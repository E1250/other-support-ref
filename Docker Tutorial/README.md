* Youtube Video - https://www.youtube.com/watch?v=pTFZFxd4hOI
## What is Docker?
A platform for building, running and shipping applications.

sometimes when you wanna share a code with others it might no work. cause of 
* One or more files are missing.
* Software version mismatch.
* Different configuration setting.

you can use one or more than docker app

## Virtual Machines vs Containers
![image](https://github.com/E1250/other-support-ref/assets/24204104/956f9224-65cf-495e-a11c-9da766145e82)

### Hypervisor
is software used to create and manage virtual machine
* VirtualBox
* VMware
* Hyper-v (Windows only)

![image](https://github.com/E1250/other-support-ref/assets/24204104/01e9d7bb-1684-4ad9-8467-cf0dfe6ef588)

### Problems
* Each VM needs a full-blown OS
* Slow to start
* Resource intensive

### Containers
* Allow running multiple apps in isolation
* Are lightweight
* Use OS of the host
* Start quickly
* Needless hardware resources

## Docker Architecture
![image](https://github.com/E1250/other-support-ref/assets/24204104/354e4f30-a0db-4207-b82b-effa20a1de87)
> **NOTE:** All containers shares the `kernel` of the host

![image](https://github.com/E1250/other-support-ref/assets/24204104/cfac7919-0417-4f8a-994f-f6f5d3a89d29)
```cmd
docker version
```

## Development Workflow
![image](https://github.com/E1250/other-support-ref/assets/24204104/3e4e2163-3bc8-4876-b9d8-2e2d09ab55d3)
### Image
* A cut-down OS
* A runtime environment (eg Node)
* Application files
* Third-party libraries
* Environment variables
  
![image](https://github.com/E1250/other-support-ref/assets/24204104/2eda6ce4-896f-4890-baae-adb5862db3c9)

## Docker in Action
### Instructions
to dockerize python file 
* Start with an OS
* Install python
* Copy app files
* Run `python app.py` file

After creating the `Dockerfile`, run
```cmd
docker build -t hello-docker .
```
now to show the docker image and other docker images
```cmd
docker images
docker image ls
```
to run docker image
```cmd
docker run image-name
```
try this out - https://labs.play-with-docker.com/p/cjepcp8gftqg00flvcrg#cjepcp8g_cjepcqggftqg00flvcs0
to use a docker image from docker hub
```cmd
docker pull usename/docker_image_name
```
## Linux Distros
* Ubunity
* Debian
* Apline
* Fedora
* CentOS

## Running Linux
```cmd
# Docker wll search about this image locally or docker will download it
docker run ubuntu

# Show running containers
docker ps -a

# Run and able to interact with, now you will see the shell
docker run -it ubuntu


```
in shell
```shell
# Print hello
echo hello

whoami

# Location of the shell program
echo $0

# Show history
history
```

## Managing Packages
* npm
* yarn
* pip
* NuGet

```cmd
apt update
apt list
apt install package-name
```
## Linux File system
![image](https://github.com/E1250/other-support-ref/assets/24204104/cb642290-ce68-41c1-86d7-bd27210ef0a5)
> Use `Tab` for autofill
```cmd
pws  # Print working directory
ls
ls -l
cd file-path
cd ..    # go one level up
cd ~   # Go to home directory
mv from to  # Moving or renaming directory from to
touch hello.txt file2.txt
ls -1
rm files.txt
rm file*
rm -r filename    # Remove directory
mkdir dirname   # Creating directory
cat filename  # show content of the file
more filename
head -n 5 filename
tail -n 5 filename
```
## Redirection
```cmd
# write data from file1 to file2
cat filename1 > filename2
```
