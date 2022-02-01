# jupyterlab-with-java-kernel
Documentation on how to install and use Java in a Jupyter Notebook


## Before starting: Installation of dependencies

### 1. Initialise the environment for use with conda

```bash
conda init zsh
exec -l. zsh
```

### 2. Create a new conda environment with the scijava-jupyter-kernel library 

The library provides a JupyterLab kernel with Java. Official documentation and the source code of the library that enables the use of Java in a jupyter notebook can be found here https://github.com/scijava/scijava-jupyter-kernel.

```
conda create --name java  scijava-jupyter-kernel -y
```

### 3. Activate the newly created Java environment

```
conda activate java
```

Now Java can be used both from the command line, to execute files, or in an interactive session using a Java Notebook. 
See below how you can access the Jupyter Kernel with Java.

#### 1. Creating a new Java Notebook

A new Java Notebook can be created by accessing the `SciJava` tile in the launcher menu.

![](http://g.recordit.co/MxiFR9TOLK.gif)

#### 2. Opening an existing Java `ipynb` notebook

When accessing an existing Java notebook, you can verify that the correct kernel (`sci-java`) has been selected by accessing the kernel dropdown in the top right corner.

![](http://g.recordit.co/FsIG9YHkzL.gif)
