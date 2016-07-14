Light Dark Matter eXperiment Conceptual Design Report
=====================================================

Requirements
------------

Building of the document requires the following tools: 
* [CMake >= 2.8](http://www.cmake.org/cmake/help/install.html)

Building the Document
---------------------

##### Clone the repository from GitHub #####

The document is stored in a public GitHub repository.  The LaTeX source can be 
"cloned" i.e. copied to a users local machine by issuing the following commands
from a terminal

    cd /path/to/workdir
    git clone https://github.com/omar-moreno/ldmx-cdr.git

A github account in not required to clone the source code, but one will be 
needed to commit any changes made to the document.

##### Generating a PDF #####

Generating a PDF copy of the document can be done as follows: 

    cd ldmx-cdr
    mkdir build; cd build
    cmake ../
    make

The document will be placed in the build directory.

Git Quick Start
---------------

##### Checking which files were modified #####
The command 

    git status

will output an overview of the files that have been modified

    # On branch master
    # Changes not staged for commit:
    #   (use "git add <file>..." to update what will be committed)
    #   (use "git checkout -- <file>..." to discard changes in working directory)
    #
    #	modified:   README.md
    #
    no changes added to commit (use "git add" and/or "git commit -a")

##### Committing changes to a file #####

Once a document has been modified, the changes can be committed as follows
    
    git add /path/to/modified/file.tex
    git commit -m "commit message"

This will only commit the changes to file.tex.  If multiple files have been 
modified, they will need to be added before committing as follows

    git add /path/to/modified/first_file.tex
    git add /path/to/modified/second_file.tex
    git commit -m "commit message"

##### Pushing changes to GitHub #####

All changes made to a document, once committed, need to be pushed to the main
repository on GitHub.  This can be done by using the following command:

    git push

This will prompt you for your GitHub username and password.

##### Links to other resources #####

* [git - the simple guide](https://rogerdudler.github.io/git-guide/)

Document Structure
------------------ 

