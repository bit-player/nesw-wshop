classtmpl
=========

A template to create class websites using pelican, on github.

pip install pelican==3.4
pip install markdown==2.4

files to edit:

pelicanconf.py	added projects	2 months ago
publishconf.py	more cname play	2 months ago
sitestuff.py

export PYTHONPATH=`pwd`

make your edits, see files in pages and posts.

you may need to edit the makefile for flowing images and other resources.

make homework 
make labs
make lectures
make other

git add .
git commit -m "commit message" -a
git push (you are pushing master)

make html 
make serve (to serve locally) on localhost:8000 

make github (uses gh-import to push to gh-pages branch)
