# Exporter Program is currently bugged 5/21

Was still trying to remove pipes from text within the gathering program. I tried to gather some more test tweets when suddenly it no longer gave tweets.
I test this the day before (5/20) and it was working just fine. I am currently unsure if it is due to my machine or the program suddenly breaking. 


# Twitter Project

Repo for Getting and Cleaning Tweets for UTK CURENT


# Getting the Repo & Setting Up
All you need to do is either clone it with Git or if you don't know Git, just download the zip file containing it all.
Install **pyquery** & **urllib2** for Python 2.7 using pip. This will need to be used in an Unix environment. 

# Getting Tweets
In the #GetProg# Folder, you'll be using Exporter.py to handle the gathering of Tweets. 
This takes a bit of time so be patentient with it all. 

It operates under several modes but the two main ones are "--username" and "--querysearch".
For most purposes, "--querysearch" is all that's needed unless you want to focus on a certain person. 

Using Unix with Python installed. Once in the directory, open a terminal and input

**python Exporter.py --COMMAND "@USERNAME"**

This will gather and store all the tweets doing this. Several instances of this program can be run at the same time. 

# Cleaning the Tweets
In the Cleaning Folder, **Main.py** will filter by date, remove unicode errors, translate (if enabled), and combine all files into a single one.

Right now the translation is commented out. To enable, please
uncomment.

To use:
cd Cleaning
cp "where the tweets files are" SepCleaning/
python MAIN.py

This works by doing a bit of hopscotch between two folders thanks to Python's CSV module. All you need to do is update path1 and path2 inside the main file and it should work. Replacing the osdir path needs to be done as well. When tested this worked on cleaning and removing all unneccessary files. 
