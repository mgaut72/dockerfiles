FROM    mgaut72/python-base

RUN     echo "deb http://ppa.launchpad.net/jon-severinsson/ffmpeg/ubuntu quantal main" >> /etc/apt/sources.list
RUN     apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 1DB8ADC1CFCA9579

RUN     apt-get update -y

RUN     apt-get install -y -q libavformat-dev libavcodec-dev libavfilter-dev libswscale-dev libjpeg-dev libpng-dev libtiff-dev libjasper-dev zlib1g-dev libopenexr-dev libxine-dev libeigen3-dev libtbb-dev libboost-python-dev curl cmake

RUN        curl -L 'http://sourceforge.net/projects/opencvlibrary/files/opencv-unix/2.4.7/opencv-2.4.7.tar.gz/' | tar xvzf - && mkdir -p opencv-2.4.7/release && cd opencv-2.4.7/release && cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local -D BUILD_PYTHON_SUPPORT=ON -D WITH_XINE=ON -D WITH_TBB=ON .. && make && make install
