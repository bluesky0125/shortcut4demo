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
    
### Code-SSD/OpenAlpr...

   - [SSD]()
   - [OpenAlpr]()
   - [face_recognition](https://github.com/ageitgey/face_recognition)
   
    pip install face_recognition
   
### Installation Validation
    $ nvcc --version
    $ nvidia-smi

