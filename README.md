``` python
import nltk
import ssl

try:
    _create_unverified_https_context = ssl._create_unverified_context
except AttributeError:
    pass
else:
    ssl._create_default_https_context = _create_unverified_https_context

nltk.download()
```

# New directions for Week 2

It's probably easiest to get the new files manually. 

First, on this page, click "clone or download" and download a
zip file. This will give you the entire contents of this repository.

Then move the relevant files to your LS_mining_course folder:

    * move notebooks 6 and 7 over.
    * move the folder "mtms_csv" from the download into the corpora folder
    * move the file named "lexicon.txt" from the download into your lists folder
    * Finally there's a pdf named "Collocations for Manning and Schuetz.pdf" that you can put wherever you want.

# Getting setup

These directions are to, a certain extent, mac specific. Linux machines will be very similar. Windows machines will be close, but will differ here and there.

## 1. Copy stuff from this github repository

A first step is to copy the material from this repository to your own computer.
On a mac, I recommend that you do this in your home directory. 

```
cd ~
git clone https://github.com/bsherin/LS_mining_course.git
```

If that doesn't seem to work, click on of the links on this page to simply
download the files.

When you're done, you should have a new folder named `LS_mining_course`.

## 2. Create your python virtual environment

Open a Terminal application and `cd` into the `LS_mining_course` folder you just created

```
cd LS_mining_course
```
Then use these commands to create the virtual environment.

```
virtualenv -p /usr/local/bin/python3 venv
source venv/bin/activate
pip install -r requirements.txt
```

## 3. Launch the jupyter notebook or jupyter lab

Steps 1 and 2 above you only have to do once. But step 3 you might need to do
whenever you start working.

First `cd` into the LS_mining_course folder

```
cd ~/LS_mining_course
```

Then activate the python virtual environment you created above

```
source venv/bin/activate
```

Finally, start the jupyter notebook

```
jupyter notebook
```

Or the jupyter lab

```
jupyter lab
```

I also created some shortcuts to make this quicker.
If you're on a mac you can double_click on jupyter_lab or jupyter_notebook.

You can also run one of these scripts:

```
sh launch_lab.sh
sh launch_notebook.sh
```

# To launch in binder:

https://mybinder.org/v2/gh/bsherin/LS_mining_course.git/master

