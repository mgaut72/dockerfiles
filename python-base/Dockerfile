FROM    ubuntu:12.10

RUN     apt-get update -y

# basic python dependancies
RUN     apt-get install -y -q build-essential python-dev python-setuptools
RUN     easy_install pip

# basic numpy/scipy dependancies
RUN     apt-get install -y -q gfortran libblas-dev libatlas-dev liblapack-dev

RUN     pip install numpy
RUN     pip install scipy
