Light Dark Matter eXperiment Conceptual Design Report
=====================================================

Requirements
------------

Building of the document requires the following tools: 
* [CMake >= 2.8](http://www.cmake.org/cmake/help/install.html)

##### Building the Document #####

###### Clone the Repository from GitHub ######

The document is stored in a public GitHub repository.  The LaTeX source can be 
"cloned" i.e. copied to a users local machine by issuing the following commands
from a terminal

    cd /path/to/workdir
    git clone https://github.com/omar-moreno/ldmx-cdr.git

A github account in not required to clone the source code, but one will be 
needed to commit any changes made to the document.

###### Generating a PDF ######

Generating a PDF copy of the document can be done as follows: 

    cd ldmx-cdr
    mkdir build; cd build
    cmake ../
    make

The document will be placed in the build directory.

##### Document Structure #####
