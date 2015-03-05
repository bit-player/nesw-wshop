classtmpl
=========

A template to create class websites using pelican, on github.

```
pip install pelican==3.4
pip install markdown==2.4
```

Do the above. Use Anaconda Python and set path accordingly. Dont edit the below.

files to edit:

* pelicanconf.py
* publishconf.py
* sitestuff.py

At the top level directory, to bring in modules, etc in support:

```
export PYTHONPATH=`pwd`
```

make your edits:

* do the ipython notebooks and a md file in which a notebook is embedded in Notebooks 
* a makefile copies both the md file and the ipython notebook from there to the content folder and its subfolders posts and notebooks
* the main concept is bloggy, so that you can run a class/whop over time
* if you need non bloggy pages look and edit them in content/pages. The index file and other files like syllabus/about/contact/schedule are all there
* all the navigation is done by MENUITEMS in pelicanconf.py. The look of index page is controlled by stuff in sitestuff.py and index.md in pages.

you may need to edit the makefile for flowing images and other resources.

```
make Notebooks

git add .
git commit -m "commit message" -a
git push (you are pushing master)

make html 
make serve (to serve locally) on localhost:8000 

make github (uses gh-import to push to gh-pages branch)
```
