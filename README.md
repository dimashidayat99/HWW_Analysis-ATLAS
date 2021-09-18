# Particle Physics Analysis Tutorials Using ATLAS 13TeV Open Data

This repository will introduce you to particle physics experiment analysis. Here, we will learn how the particle physics analysis work using programming (yes of course, particle physics analysis use programming!). 

Below, I had listed the "things" that is needed before we start on the tutorial.

## Linux

Most of us use the Windows Operating System (OS), there are another OS that we will be mainly use in particle physics analyses which is Linux or Unix (Different thing !). First thing to do is like exactly what you think which is we need Linux in our computer. Well it doesnt means that we need to change our OS. There is a software that can be use called as Ubuntu which have function similiar like Linux.

### Ubuntu

Ubuntu is the modern, open source operating system on Linux for the enterprise server, desktop, cloud, and IoT. In simple words, Ubuntu is a free operating system that uses the Linux kernel. There is two places where we can install the Ubuntu (**LTS version**). You can download the Ubuntu in the [Ubuntu Official Website](https://ubuntu.com/download/desktop). You also can download the Ubuntu in the Microsoft Store. Install the Ubuntu, open it and then we will ready to go to the next part.

## GitHub

GitHub is a Git repository hosting service. It is a provider of Internet hosting for software development and version control using Git. It offers the distributed version control and source code management functionality of Git, plus its own features. In simple word, it is a place on the internet where we can sharing a code/script with other people. Usually, we will working with many people on the same script. Therefore, to make sure everything on the script is "sync", we will use the GitHub. 

The next step is copy all content of the tutorials by click on `code` on the this GitHub page and copy the link. Then, use this command on the Ubuntu terminal.

```bash
git clone <link>
```
Where the <link> is link that you copied. Now, we have the contents of tutorial on our computer. Next, we will continue to the next section.

## Anaconda

Anaconda is a distribution of the Python and R programming languages for scientific computing, that aims to simplify package management and deployment. We will use Anaconda to setup and use the conda environments. The conda environments is a separate place you can mess around without interupting or corrupting your default setup. 

Next things to do is as follows:

1. Install [Anaconda](https://docs.anaconda.com/anaconda/install/) using the Ubuntu terminal, use the Anaconda for Linux to install Anaconda in Ubuntu. For the tutorial please use this [link](https://phoenixnap.com/kb/how-to-install-anaconda-ubuntu-18-04-or-20-04).
2. Setup a Conda environment first and use it.

Before setup the Conda environment, please make sure now we are on `base` environment. If you are not in the `base` try to use this command and please specify your own directory e.g. change `username` to you own path.
```bash
eval "$(/home/username/anaconda3/bin/conda shell.bash hook)"
```
To setup the Conda environment.

```bash
conda create -n root_env
```
where the `root_env` is the Conda environment that we created (You also can change the `root_env` to different name but now just follow me). Depending what you need to install in the environment, you may change the environment name depends on you.

To enter the Conda environment and exit the Conda environment.

```bash
conda activate root_env #enter
conda deactivate root_env #exit
```
Enter the environment. Because the environment is empty, we need to install the package even that the base/default environment has all the package. Install this package.

```bash
conda install ipykernel
conda install notebook
```
Next, we will install the ROOT. Since the ROOT is quite long to install, we will install it first without knowing what it is. Later in the section below, we will have a brief explaination about ROOT. To install the ROOT.

```bash
conda install -c conda-forge root
```
Waiting for ROOT to install, let's have a read to the next section.

### Jupyter Notebook

The Jupyter Notebook is an open source web application that allows editing and running notebook documents via a web browser. We will use Jupyter notebook to run the particle physics analysis later. Since we already install the notebook in our `root_env`, just run the Jupyter Notebook.

```bash
Jupyter-notebook
```
Then, we will be given the link, just copy and paste to the browser and done. Finally, our preparation is complete.

## C++ and Python

Both language C++ and python can be used in the particle phsyics data analysis. However, the C++ is the main programming languange in the particle physiscs. Even in this tutorial, we will use mainly this languange for the data analysis. In this tutorial, there is no requirement to learn these two language before we start but it is better for you to explore this language for your future because now most of courses in the university will learn how to coding and most of the company need people who can coding. Therefore, I will give some link for you to explore.

* [C++ Tutorial Documentation](https://www.cplusplus.com/doc/tutorial/)
* [C++ Tutorial Youtube](https://www.youtube.com/watch?v=vLnPwxZdW4Y&vl=en)
* [Python Tutorial Documentation](https://docs.python.org/3/tutorial/)
* [Python Tutorial Youtube](https://www.youtube.com/watch?v=_uQrJ0TkZlc&vl=en)
* [C++,Python,ROOT Tutorial GitHub](https://github.com/afyqazraei/MalayaHEPTutorials)

## ROOT

ROOT is data analysis framework for particle physics which is developed by CERN. The ROOT is the main framework that we will use in this tutorial. This framework is very powerfull and likely will be used in most experimental particle physics. There is a lot things to explore with ROOT. You may want to explore the [ROOT Tutorials](https://root.cern/doc/master/group__Tutorials.html).
