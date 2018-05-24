### Versions
    Ubuntu 16.0.4, Cuda8.0, CuDnn6.0, tensorflow1.3.0, python2.7, pyqt5, spyder, dlib19.12,opencv2.4.9.1 ...
### Packages

    cuda   
    $ sudo apt-get update
    $ sudo apt-get install nvidia-cuda-toolkit
    $ sudo apt install nvidia-cuda-dev
    $ sudo apt-get -y install cuda-8-0
    $ sudo apt-get upgrade
    $ vim ~/.bashrc
    export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/cuda/lib64/
       
    python-repos
    $ sudo apt-get install python-opencv
    $ sudo apt-get install python-pip
    $ sudo apt-get install python-pyqt5
    $ sudo pip install spyder
    
    pip
    $ wget https://bootstrap.pypa.io/get-pip.py
    $ sudo python get-pip.py
    
    dlib-cmd
    $ sudo apt-get install build-essential cmake libgtk-3-dev libboost-all-dev
    $ sudo pip install numpy scipy scikit-image dlib
    
    dlib-build
    $ wget http://dlib.net/files/dlib-19.12.tar.bz2
    $ tar xvf dlib-19.12.tar.bz2
    #$ cd dlib-19.12/
    #$ mkdir build
    #$ cd build
    #$ cmake ..
    #$ cmake --build . --config Release
    #$ sudo make install
    #$ sudo ldconfig
    #$ cd ..
    $ cd dlib-19.12
    $ python setup.py install
    #$ rm -rf dist
    #$ rm -rf tool/python/build
    #$ rm python_examples/dlib.so
    #$ pip install dlib

    tensorflow
    $ pip install -U tensorflow-gpu==1.3.0
    
    enum
    $ pip install pyOpenSSL service_identity enum
    
    pyqt5
    $ sudo apt install python-pyqt5
    
    spyder
    $ sudo pip install spyder
    
    
### Code-SSD/OpenAlpr...

   - [SSD]()
   
    $ git clone http://github.com/gustavkkk/surveillance-system.git
    $ cd surveillance-system
    $ mkdir checkpoints
    $ curl -o ssd_300_vgg.ckpt.zip https://raw.githubusercontent.com/balancap/SSD-Tensorflow/master/checkpoints/ssd_300_vgg.ckpt.zip
    $ unzip ssd_300_vgg.ckpt.zip checkpoints
   
   - [OpenAlpr](https://github.com/openalpr/openalpr/issues/660)
   
    $ sudo apt-get install libopencv-dev libtesseract-dev git cmake build-essential libleptonica-dev
    $ sudo apt-get install liblog4cplus-dev libcurl3-dev
    # If using the daemon, install beanstalkd
    $ sudo apt-get install beanstalkd
    # Clone the latest code from GitHub
    $ git clone https://github.com/openalpr/openalpr.git
    # Setup the build directory
    $ cd openalpr/src
    $ mkdir build
    $ cd build
    # setup the compile environment
    $ cmake -DCMAKE_INSTALL_PREFIX:PATH=/usr -DCMAKE_INSTALL_SYSCONFDIR:PATH=/etc ..
    # compile the library
    $ make
    # Install the binaries/libraries to your local system (prefix is /usr)
    $ sudo make install
    # Test the library
    $ wget http://plates.openalpr.com/h786poj.jpg -O lp.jpg
    $ alpr lp.jpg
    $ cd ../src/binding/python
    $ python setup.py install
    
   - [face_recognition](https://github.com/ageitgey/face_recognition)
   
    $ sudo pip install face_recognition==1.2.2
   
### Installation Validation
    $ nvcc --version
    $ nvidia-smi

