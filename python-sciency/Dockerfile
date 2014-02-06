FROM    mgaut72/python-base

RUN     apt-get update -y

# numpy dependancies
RUN     apt-get install -y -q gfortran libblas-dev libatlas-dev liblapack-dev libfreetype6-dev libpng-dev

RUN     pip install numpy
RUN     pip install scipy
RUN     pip install matplotlib
