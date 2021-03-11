# Instalación de Python

Python se encuentra disponible para las diferentes sistemas operativos del mercado (Windows, Linux, MacOs, etc).

Anaconda nos permite instalar python de forma amigable, nos brinda un entorno desarrollo completo con la posibilidad de integrar distintos complementos de forma rapida y facil.

Se procedera a detallar los pasos necesarios para instalar miniaconda que es una versión reducida de anaconda para los sistemas operativos Windows y Linux.

Para mayor información sobre anaconda puede consultar el siguiente enlace: [link](https://docs.conda.io/en/latest/index.html)

## Windows

La siguiente instalación se realizara mediante el uso del terminal de windows, el motivo es permitir familiarización del uso de la terminal y sus comandos basicos.

Usamos la combinación de teclas "win+r", que abrira el ejecutador y escribiremos "cmd" como se aprecia en la siguiente figura:

![fig1](https://github.com/oolaya1815/variados/blob/main/python/images/install1.JPG)

En el terminal ejecutamos 

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

## Configurando el entorno 

Procedemos a crear un entorno virtual con python en su versión 3.7 y Tensorflow en su versión 2.1

```
conda create --name tensorflow python=3.7
conda activate tensorflow
```

Instalando Tensorflow con soporte solo a CPU

```
conda install -c anaconda tensorflow
```

Instalando Tensorflow con soporte a GPU

```
conda install -c anaconda tensorflow-gpu
```

Instalando dependencias y librerias

```
conda env update --file tools.yml
```
