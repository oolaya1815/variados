
# Python installation

Python is available for the different operating systems on the market (Windows, Linux, MacOs, etc).

Anaconda allows us to install Python in a friendly way, it gives us a complete development environment with the possibility of integrating different add-ons quickly and easily.

We will proceed to detail the necessary steps to install miniaconda which is a reduced version of anaconda for Windows and Linux operating systems.

For more information about anaconda you can consult the following link: [link](https://docs.conda.io/en/latest/index.html)

## Windows

The following installation will be made by means of the use of the terminal of windows, the reason is to allow familiarization of the use of the terminal and its basic commands.

We use the combination of keys "win+r", that will open the executor and we will write "cmd" as it is appreciated in the following figure:

![fig1](https://github.com/oolaya1815/variados/blob/main/python/images/install1.JPG)

In the terminal run 

```
curl https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.exe --output miniconda.exe
```

Procedemos con la instalación

```
miniconda.exe
```


## Linux

```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
```

## Setting up the environment 

We proceed to create a virtual environment with python version 3.7 and Tensorflow version 2.1.

```
conda create --name tensorflow python=3.7
conda activate tensorflow
```

Installing Tensorflow with CPU-only support

```
conda install -c anaconda tensorflow
```

Installing Tensorflow with GPU support


```
conda install -c anaconda tensorflow-gpu
```

Installing dependencies and libraries


```
conda env update --file tools.yml
```
