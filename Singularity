#######################################################################################
## DO NOT EDIT THIS FILE! This file was automatically generated from the dockerfile. ##
## Run babelwhale::convert_dockerfile_to_singularityrecipe() to update this file.    ##
#######################################################################################

Bootstrap: shub

From: dynverse/dynwrap:py3.6

%labels
    version 0.1.3

%files
    . /code

%post
    chmod -R 755 '/code'
    pip install python-igraph louvain 
    pip install feather-format
    pip install scanpy
    pip install fa2

%runscript
    exec python /code/run.py

