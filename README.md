#IPython Research Notebook by Mikhail Klassen

##Description 
The IPython notebook is an ideal tool for keeping track of your research because
it allows you to mix your analysis code with inline figures and comments. At the
start of the day, you can open a fresh notebook and type up your research
progress over the course of the day. Use the notebook environment to write up
your analysis scripts and produce figures on the fly. Combine programming with
documenting in one fluid, stream-of-consciousness process.

##Requirements 
This tool currently consists of a `bash` script and a template.  It is intended
to be run within a UNIX command-line environment. Your system must already have
`python`, `IPython`, and `IPython notebook` installed in order to use this tool.
For inline analysis and visualization, you may also want to install `numpy`,
`scipy`, `matplotlib`, and `pandas`. 

##Installation 
Assuming you have all the system requirements, simply clone the repository to
set up your research notebook environment.

`git clone git@github.com:mikhailklassen/IPython-Research-Notebook.git`

##Usage 
To add an entry for today, run the `add_entry` script.

`./add_entry`

This should create a folder for the current year and copy the template entry
from `./templates/entry.ipynb` to the "year" folder. The copied template entry
is renamed to match today's date. The IPython notebook webserver should be
launched immediately, and your browser opened to the dashboard. 

###HTML Bundler 
You can simply run the `make_html` script to generate a tarball
containing all of your ipython notebooks as well as an index.html linking to
them through the wonderful js [nbviewer](https://github.com/ipython/nbviewer).
You can then just dump this into a directory on your webserver and your
notebooks are viewable using some simple static html.

##Acknowledgements 
Kudos goes to [Ben Keller](https://github.com/bwkeller) for convincing me to
switch to the IPython notebook for my research note-taking.
