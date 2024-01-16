CLASS_AniEDE: Cosmic Linear Anisotropy Solving System for the Anisotropic EDE Model
==============================================

Authors: Vivian Sabla (& Robert Caldwell)

This is a fork of the Einstein-Boltzmann solver CLASS written by Julien Lesgourgues,
Thomas Tram, Nils Schoeneberg, et al.; refer to the original repository for the README of CLASS.
For download and information on original code, see http://class-code.net

All modifications to the original CLASS code are marked with a comment containing 'AniEDE mod'.

The Anisotropic EDE Model
-------------------------

This model is a specific case of the phenomenological generalized model of EDE 
presented in Sabla et al. (2022): https://arxiv.org/pdf/2202.08291.pdf.



[ ADD IN DETAILS OF MODEL ] 

Compiling CLASS_AniEDE and getting started
------------------------------------------

To install, clone this repository from the terminal and run:
    cd class_ani-ede
    make clean
    make
To avoid conflicts with other builds of CLASS, it is recommended that you 
do the above in a new virtual environment. 

Note: To use CLASS from python, or ipython notebooks, or from the Monte
Python parameter extraction code, you need to compile not only the
code, but also its python wrapper. This can be done by typing just
'make' instead of 'make class' (or for speeding up: 'make -j').
I've found that on some machines make sure to separately compile the python code if 
planning on using the python wrapper.
To do this, within the class_ani-ede directory do:
    cd python
    python setup.py install --user
Make sure your path to your C compiler is correct 
(see: https://github.com/lesgourg/class_public/issues/462). 

To check that the code runs:
    ./class explanatory_AniEDE.ini
If the above runs with no error, you have succeeded. 

Usage
-----

To run you need a .ini file. An example is given with explanatory_AniEDE.ini. 

[ ADD IN DETAILS OF MODEL ]

If you use this code, please ... 

Support
-------

If you have issues, please feel free to contact me at vivian.iossa.sabla@gmail.com. 
