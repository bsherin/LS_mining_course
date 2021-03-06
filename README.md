# For week 9

All of the notebooks that start with **W9**. 

Plus you'll want the folder **network_data**.

You can also download and install Gephi (https://gephi.org). We'll be using it to view some networks.

# For week 8

Just all of the notebooks that start with **w8**.

# For week 7

Get the notebooks that start with **W7**.

And there are two new libraries to install:

* pyldavis
* wikipediaapi

# For week 6

Get the notebooks that start with **W6**.

One new list: 

* stoplist3k2sw.txt

One new corpus file: 

* student_questions.txt

# For week 5

There is a new numbering scheme for notebooks. You want all of the notebooks that start with **W5**.

From the **corpora** folder you should grab these folders:

* bernstein_all
* encoding_test_files

And these files:

* mtms2008-09-122a.pdf
* tekno_fractions_nona.xlsx
* single_arg_page.html

# For week 4

You want **notebooks 12-16**. 

You can also grab my version of last week's solo work, if you're interested. It's **11 - Solo word 3-BS.ipynb**

The new **corpus files** for this week are:

* male.txt
* female.txt
* pizza.csv
* tekno_flat.csv

Grab the **images folder** and it's contents.

Grab two **journal articles** I uploaded, if you're interested.

* Landauer (an introduction to LSA)
* Kersting (an article about Tekno, which is the project associated with a corpus you'll work with)

# For week 3

You want notebooks 8, 9, 10, and 11. Put those in your LS_mining_course folder.

There's a new list in the lists folder called "seasons_stop_list.txt." Put that in your lists folder.

There are two new sub-folders in the corpora folder that you should grab. 
They are called "seasons" and "seasonscomparisondoc."

Finally, to do the nice printing of matrices you need to install the sympy python package.

Also, you need to grab two modules. seasons_module.py and uttilities.py

```
source venv/bin/activate
pip install sympy
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

https://mybinder.org/v2/gh/bsherin/LS_mining_course.git/master?urlpath=lab

