# Installing Jupyter Lab locally
(Originally developed by [Suresh](https://github.com/suresh-sitharaman/ai-training/tree/main) )

You can install and run Jupyter notebooks locally in your machine, if you prefer. We will provide two means of installing the notebook.

## Jupyter Lab Installation - Approach 1
If you already have *Python3* installed in your machine, then follow the instructions in this section
For running the lab notebooks, we recommend python version of *v3.10.x* but any version above *v3.7.x* should work just fine. Please check your current installed version by running the following command:

             python3 -V

And as long as it satisfies the requirement mentioned previously, you are good to go.
It is recommended that you install Jupyter Lab in a python virtual environment so that the python libraries that you install during the lab sessions do not conflict with  any other application dependencies that you might have in your machine. 

Follow the following instructions to do this:
- Create a directory called **jupyter_lab** and change (cd) into that directory​
- Run the following command to create a virtual environment called jupyter_lab (you can name the environment anything you want):
 
        python3 –m venv jupyter_lab

- To activate the newly created virtual environment, run the command (if you used a different name while creating the virtual environment, then use that name below instead of jupyter_lab): 

        source jupyter_lab/bin/activate 
You can now install the Jupyter Lab in your machine by executing the following command:

            pip3 install jupyterlab
Wait for the installation to complete. To start the application, run the following command:

            jupyter lab
This will automatically open the application in your default browser on port 8888

## Jupyter Lab Installation - Approach 2
If you do not have python installed in your machine, then we recommend the approach described in this section to install Jupyter Lab. We recommend using [Miniconda][miniconda] which is a minimal distribution containing Python and [conda][conda], an open source package and environment manager that helps with *install, update and removal* of python packages.

Following are the steps to install Miniconda
- Start by visting the [download][mdownload] page
- Depending on your operating system, choose the appropriate (**32-bit or 64-bit**) installation version for python version 3.10 (files will be named *Miniconda3-py310_xxx*) and download it to your machine
- Go to your download directory and double-click on the installation file. Follow the instructions on the screen
- During the installation, you will be prompted whether to install the app for **Just Me** or **All Users**. We recommend you pick **Just Me**, but we leave it up to you. You must have *Admin privilege* in your machine to install for **All Users**

After the installation is complete, check to make sure that **conda** is installed correctly.
For Mac/Linux machines, open a bash/zsh terminal and run the command: ​

             conda --version​

This should print out the version, something like *conda 4.9.2 (for example)*

For Windows machine, do the following:​

- Go to the Start menu and search for Anaconda Prompt (this is the Command Line Interface)​
- Click on the CLI. This will open a shell​
- In the shell, enter conda --version. This should print out the version​

We are now ready to install Jupyter Lab.

In the bash/zsh terminal (or CLI shell for Windows), enter the following:​

         conda install -c conda-forge jupyterlab

Once the installation is complete, you can start the application by running the command:

         jupyter lab
This will automatically open the application in your default browser on port 8888

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [miniconda]: <https://docs.anaconda.com/miniconda/>
   [conda]: <https://anaconda.org/anaconda/conda/>
   [mdownload]: < https://repo.anaconda.com/miniconda/>
