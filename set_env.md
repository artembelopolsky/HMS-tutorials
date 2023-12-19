---
title: Set up environment
layout: home
---


# Anaconda Navigator vs Anaconda prompt
You have probably noticed that you now have several apps installed. One of them, *Anaconda Navigator*, is a graphical interface to manage your apps and environments. However, it is quite slow and not handy, and thus should be avoided. Instead, you should use *Anaconda prompt*, which looks like a terminal window and allows to flexibly interact with Anaconda,

# Launch Anaconda prompt
Locate Anaconda prompt among your installed programs and launch it. It should look like this:
![Anaconda Prompt](/images/anacondaPrompt.png)

# Create your own environment
You can see on the image above that you are in a default environment called *base* environment. You should avoid using it and instead create your own environment, specific to your project needs.

To create a new environment called *default* (feel free to give it another name):

```
conda create -n "default"
```

This environment will come with the version of python you have selected during installation of *Anaconda*. Sometimes, you may want to choose a different version of python for your own environment:

```
conda create -n "default" python=3.7.0
```
If you know you may need certain packages (e.g., matplotlib for plotting), you can immediately install them here as well, like so:

```
conda create -n "default" python=3.7.0 matplotlib
```


# Activate your environment
In order to use your environment, you need to activate it:

```
conda activate default
```

You will notice that the *(base)* prefix will change to *(default)*

# Installing Spyder as IDE

In order to start programming, we need an *Integrated Development Environment* or *IDE*. Below we install *Spyder* as our IDE. Spyder is another package that we can install in our environment. Our package manager (*conda*) takes care to choose the right package that does not conflict with our environment.

```
conda install spyder
```

# Launch Spyder

Now we can launch Spyder and start programming.
![launch Spyder](/images/launchSpyder.png)


