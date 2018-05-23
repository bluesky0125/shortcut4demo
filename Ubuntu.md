### Versions
    Ubuntu 16.0.4, Cuda8.0, CuDnn6.0, tensorflow1.3.0, python2.7, pyqt5, spyder, opencv2.4.9.1 ...
### Packages

   - [cuda](https://github.com/michael0125/shortcut4demo/blob/master/install-cuda.sh)
   
    $ sudo apt-get update
    $ sudo apt-get install nvidia-cuda-toolkit
    $ sudo apt-get upgrade
    
   - [cudnn](https://github.com/michael0125/shortcut4demo/blob/master/install-cudnn.sh)
    
    python-repos
    $ sudo apt-get install python-opencv
    $ sudo apt-get install python-pip
    $ sudo apt-get install python-pyqt5
    $ sudo pip install spyder
    
    pip
    $ wget https://bootstrap.pypa.io/get-pip.py
    $ sudo python get-pip.py
    
    dlib
    $ sudo apt-get install build-essential cmake
    $ sudo apt-get install libgtk-3-dev
    $ sudo apt-get install libboost-all-dev
    
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

