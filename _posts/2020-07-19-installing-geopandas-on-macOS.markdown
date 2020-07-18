---
layout: post
title:  "Installing GeoPandas, macOS"
date:   2020-07-19 06:01:53 -0700
categories: GeoPandas
tags: [python, mapping, gis, macOS, windows10, win10]

custom-css-list:
     - slider/image-slider.css
---
I'm currently creating maps using the Python package [GeoPandas](https://geopandas.org/index.html){:target="_blank"}.  GeoPandas is an open 
source Python package that, once installed, is pretty easy to use; at least it 
was easy for me, who had very little GIS experience but am an intermediate 
coder. It relies heavily on Pandas and MatPlotLib libraries.  

I think the biggest learning curve for novice coders will be understanding and 
using data frames with Pandas.  It's worth spending some time understanding 
how data frames work, and how to call data subsets, but that's a post (or 
workshop) for another day.

Before you can use GeoPandas, you need to install it.  Installation on macOS 
is fairly easy, but installing on Windows 10 made me want to throw my Win10 
laptop out a window.  I didn't, but I really wanted to. If I had not already 
had an early success with GeoPandas on my Mac laptop, I would have given up!  Don't 
give up!  There is a way to install GeoPandas and start creating maps.


## Installing GeoPandas (Mac) 

I was able to install GeoPandas on my Mac using the first command on their 
[installation page](https://geopandas.org/install.html){:target="_blank"} - `conda install geopandas` - 
but I knew I already had almost all of the dependencies installed.  If 
you're not sure if you have dependencies installed, try using the following.

1. Make sure conda is available through the terminal.  You can do this by 
opening a terminal and executing

        conda --version  

    Note the double-dash before `version`  If you recieve a response similar to 

        conda 4.8.3

    you're good to go, and can skip down to #N.  

    If you receive

        command not found 

    response, continue to #2.

2.  Do you have conda installed on your computer?  I have it installed through 
Anaconda. If you do not have conda installed on your computer, install 
it.  For newcomers, I recommend [Anaconda](https://www.anaconda.com){:target="_blank"}. 

3.  If conda is installed, but typing `conda --version` results in 
`command not found`, you need to add conda to your BASH Profile.  This is 
also sometimes called adding conda to your PATH.  Basically, you're telling 
the computer where a program is so it can execute from whatever folder you 
happen to be in when you try to run it.
    
    To add it to your BASH Profile (`~/.bash_profile`), execute

        export PATH="/path/to/your/anaconda/bin:$PATH"

    if you don't know the path to your anaconda, execute 

        which python

    which will respond with the PATH to the conda executable.

    Once you've added the path to your BASH profile, double-check it's working 
    by executing

        conda --version

4.  Once you know conda is working from the terminal, execute
       
        conda install geopandas

    Your terminal will start showing lots of lines of text.  That's GeoPandas 
    being installed.  It took ~5-10 minutes (if I recall).  You'll see a 
    "success" message followed by the command prompt once it's installed.

    I needed to install two other libraries for GeoPandas to map properly. I 
    say this now because I didn't realize I needed them and they weren't 
    installed until I tried making a map in Jupyter Notebook.  So, go ahead 
    and install the following two libraries if you want to make maps with 
    GeoPandas.
  
    - decartes
    - mapclassify<br><br>
     

    Install libraries by executing 

        conda install library-name

    If a library is already installed, but needs to be updated, do so by executing

        conda update library-name


---
---
<br>
That should be it for macOS.  If you want to test it out and jump right into 
mapping, try GeoPandas [Making Maps](https://geopandas.org/mapping.html){:target="_blank"} 
doc page.

Happy mapping!
