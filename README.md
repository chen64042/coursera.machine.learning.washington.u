# coursera.machine.learning.washington.u
Homework from Machine Learning Courses Offered by Washington U

## Environment
These were done in Anaconda 3, Python 2.7 environment. I didn't follow the instructions exactly as the version of Anaconda provided in the package was too old. The following was what I did *(MacOS 10.13.6)*: 

### Setting Up Environment
* Go to [GraphLab site](https://turi.com/download/install-graphlab-create.html) and download GraphLab Create Launcher
* Request [Acedamic License](https://turi.com/download/academic.html)
* Install the downloaded package. This will install Anaconda 2, create an Anaconda 2 environmet called gl-env
* Open a terminal, type `source activate gl-env` to enter gl-env environment

#### The following steps must be execuated when gl-env is active.
* Upgrade pip `conda update pip`
* Install the license `pip install --upgrade --no-cache-dir https://get.graphlab.com/GraphLab-Create/2.1/[Your Email Address]/[Your License Code]/GraphLab-Create-License.tar.gz`
* Install Jupyter Notebook `conda install ipython-notebook`
* Install graphlab-create package `conda install -c derickl graphlab-create`. Maybe I didn't do it right but the launcher doesn't install the package for me and I have to install this manually. I have tried to repeat this process a few times and it always turns out that I must install this manually

### Setting up Anaconda 3
* Download [Anaconda 3](https://www.anaconda.com/download/#macos). Choose the one for Python 3.
* Install Anaconda 3. It should create ../anaconda3 directory under your home directory.
* Launch Anaconda 3.
* Go to *Environments*
* Select *gl-env*. This may take a few seconds
* Clone *gl-env*. Choose a new name for the cloned environment. This can take a while.
* Remove anaconda 2 installation through the terminal. `rm -Rf /home/[username]/anaconda`

### Test Your Cloned Environment
* On Anaconda 3, launch Jupyter Notebook
* Open a python notebook provided from the class.
* Make sure you don't see any errors.
* On Python Notebook, go to "Cells -> Run All"
* Make sure you see the output.

### Troubleshooting
* For some reason I got Server Error after I removed the old environment. I figured out how to fix it manually.
* Open a terminal.
* Type `which conda` to make sure you're operating under Anaconda 3 profile. (Anaconda should have created a `.bash_profile` under your home directory and prefix the PATH variable with Anaconda 3)
* Activate your cloned environment. `source activate [Your Cloned Environment Name]`
* Install ipykernal `python -m ipykernel install --user`. I keep getting server error and this is how I resolve it. This happens when you remove an environment but Anaconda is still pointing to it.

