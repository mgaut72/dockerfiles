FROM    mgaut72/python-base

RUN     apt-get update -y

RUN     apt-get install -y -q libavformat-dev libavcodec-dev libavfilter-dev libswscale-dev libjpeg-dev libpng-dev libtiff-dev libjasper-dev zlib1g-dev libopenexr-dev libxine-dev libeigen3-dev libtbb-dev libboost-python-dev curl

RUN        curl -L 'http://sourceforge.net/projects/opencvlibrary/files/opencv-unix/2.4.7/opencv-2.4.7.tar.gz/' | tar xvzf - && mkdir -p opencv-2.4.7/release && cd opencv-2.4.7/release && cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local -D BUILD_PYTHON_SUPPORT=ON -D WITH_XINE=ON -D WITH_TBB=ON .. && make && make install && cd / && rm -rf opencv-2.4.7
