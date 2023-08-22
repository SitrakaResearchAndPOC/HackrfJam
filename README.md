# HackrfJam tested with UBUNTU 20.04.1
```
apt update
```
```
apt-get install libjeromq-java libzmq-ffi-perl libzmq-java libzmq-java-doc libzmq-jni libzmq3-dev libzmq5 libzmqpp-dev libzmqpp4 python3-zmq python3-zmq libboost-dev libpython3.8-dev cmake build-essential python3-qwt python3-guiqwt python3-pyqt5.qwt libgmp-dev libxi-dev libcppunit-dev libx11-6 libx11-dev flex libncurses5 libncurses5-dev libncursesw6 libpcsclite-dev libsdl1.2-dev zlib1g-dev libmpfr6 libmpc3 lemon aptitude libtinfo-dev libtool shtool autoconf git-core pkg-config make libmpfr-dev python-cheetah libmpc-dev libtalloc-dev libfftw3-dev libgnutls28-dev libtool-bin python-lxml libxml2-dev python-sip sofia-sip-bin libsofia-sip-ua-dev sofia-sip-bin bison libgmp3-dev alsa-oss asn1c libdbd-sqlite3 libboost-all-dev libusb-1.0-0-dev python-mako python3-mako doxygen python-docutils cmake build-essential g++ python-numpy python3-numpy swig libsqlite3-dev libi2c-dev libwxgtk3.0-gtk3-dev freeglut3-dev composer phpunit python3-pip libfontconfig1-dev libxrender-dev python-sip-dev  libusb-dev libusb-1.0.0-dev libcomedi-dev libzmq3-dev javascript-common libjs-jquery libjs-sphinxdoc libjs-underscore python-sphinx-click-doc python-sphinx-copybutton-doc python-sphinx-feature-classification-doc python-sphinx-gallery-doc python-sphinxcontrib.bibtex-doc python-sphinxcontrib.programoutput-doc python-sphinxcontrib.spelling-doc build-essential libgmp-dev libx11-6 libx11-dev flex libncurses5 libncurses5-dev libncursesw6 libpcsclite-dev zlib1g-dev libmpfr6 libmpc3 lemon aptitude libtinfo-dev libtool shtool autoconf git-core pkg-config make libmpfr-dev libmpc-dev libtalloc-dev libfftw3-dev libgnutls28-dev  libtool-bin libxml2-dev sofia-sip-bin libsofia-sip-ua-dev sofia-sip-bin bison libgmp3-dev alsa-oss asn1c libdbd-sqlite3 libboost-all-dev libusb-1.0-0-dev python-mako python3-mako doxygen python-docutils cmake build-essential g++ python-numpy python3-numpy swig libsqlite3-dev libi2c-dev libwxgtk3.0-gtk3-dev freeglut3-dev composer phpunit python3-pip
```
# Installing UHD
```
git clone https://github.com/ettusresearch/uhd
```
```
cd uhd/
```
```
git checkout aea0e2de34803d5ea8f25d7cf2fb08f4ab9d43f0
```
```
cd ..
```
```
zip -r uhd.zip uhd
```
```
cd uhd/host/ && mkdir build && cd build/
```
```
cmake ..
```
```
make
```
make test
```
make install
```
```
ldconfig
```
```
cd ../../..
```
```
/usr/local/lib/uhd/utils/uhd_images_downloader.py
```

# Installing SoapySDR
```
git clone https://github.com/pothosware/SoapySDR
```
```
cd SoapySDR/
```
```
git checkout f722f9ce5b629c3c44401a9bf628b3f8e67a9695
```
```
cd ..
```
```
zip -r SoapySDR.zip SoapySDR/
```
```
cd SoapySDR && mkdir build && cd build
```
```
cmake ..
```
```
make
```
```
make install
```
```
ldconfig
```
```
cd ../..
```

#  INSTALLING GRC 38 + CLEVER JAM
```
sudo apt-get -y install autoconf automake build-essential ccache cmake cpufrequtils doxygen ethtool fort77 g++ gir1.2-gtk-3.0 git gobject-introspection gpsd gpsd-clients inetutils-tools libasound2-dev libboost-all-dev libcomedi-dev libcppunit-dev libfftw3-bin libfftw3-dev libfftw3-doc libfontconfig1-dev libgmp-dev libgps-dev libgsl-dev liblog4cpp5-dev libncurses5 libncurses5-dev libpulse-dev libqt5opengl5-dev libqwt-qt5-dev libsdl1.2-dev libtool libudev-dev libusb-1.0-0 libusb-1.0-0-dev libusb-dev libxi-dev libxrender-dev libzmq3-dev libzmq5 ncurses-bin python3-cheetah python3-click python3-click-plugins python3-click-threading python3-dev python3-docutils python3-gi python3-gi-cairo python3-gps python3-lxml python3-mako python3-numpy python3-numpy-dbg python3-opengl python3-pyqt5 python3-requests python3-scipy python3-setuptools python3-six python3-sphinx python3-yaml python3-zmq python3-ruamel.yaml swig wget
```
```
sudo apt-get install git cmake g++ libboost-all-dev libgmp-dev swig python3-numpy  python3-mako python3-sphinx python3-lxml doxygen libfftw3-dev  libsdl1.2-dev libgsl-dev libqwt-qt5-dev libqt5opengl5-dev python3-pyqt5  liblog4cpp5-dev libzmq3-dev python3-yaml python3-click python3-click-plugins python3-zmq python3-scipy python3-gi python3-gi-cairo gir1.2-gtk-3.0 libcodec2-dev libgsm1-dev libusb-1.0-0 libusb-1.0-0-dev libudev-dev
```
git log --since="2022-1-1" --until="2022-1-30"  
git log --since="2021-1-1" --until="2021-1-10"  
BEST PRECAUTION : 
* https://wiki.gnuradio.org/index.php?title=ModuleNotFoundError#B._Finding_the_Python_library
* https://wiki.gnuradio.org/index.php/UbuntuInstall

  
THE VARIABLE HAS RED CROSS IN GRC, IT IS NOT ERROR ON UBUNTU 
INSTALLING DEPENDENCIES + GNURADIO USING maint version + LOOK THE DATE  
FINDING GR-OSMOSDR COMPATIBLE WITH GNURADIO + NEAR (<) THE DATE  
ALL DEVICES (HACKRF) SHOULD BE NEAR (<) THE DATE OF GR-OSMOSDR  


COMPILING BY ORDER :   
DRIVER DEVICES -> SOAPYSDR -> SOAPYHACKRF ->  SOAPY_UHD -> GR-OSMOSDR 
hackrf 10/12/2020 < 11/01/2021 :  
61a06b904dbf5e54da1d84473004db0472950487  
soapyhackrf 21/08/2020 < 11/01/2021 : 
soapyhackrf : 7d530872f96c1cbe0ed62617c32c48ce7e103e1d 
gr-osmosdr 11/01/2021 : cffef690f29e0793cd2d6c5d028c0c929115f0ac  
INSTALLING GNURADIO maint-3.8 DATE :  
1Fevrier 2022 : maint-3.8 or 57bd109d5f0afdf09a3a52e226f464e8a71c5b82  

## INSTALLING GRC38
```
mkdir grc38
```
```
cd grc38
```
```
git clone https://github.com/mossmann/hackrf.git
```
```
mv hackrf hackrf_grc38
```
```
cd hackrf_grc38
```
```
git checkout 61a06b904dbf5e54da1d84473004db0472950487
```
```
cd ..
```
```
zip -r hackrf_grc38.zip hackrf_grc38
```
```
cd hackrf_grc38/host && mkdir build && cd build
```
```
cmake ..
```
```
make
```
```
make install
```
```
ldconfig
```
```
cd ../../..
```

## Installing SoapyHACKRF
```
git clone https://github.com/pothosware/SoapyHackRF.git
```
```
cd SoapyHackRF/
```
```
git checkout 7d530872f96c1cbe0ed62617c32c48ce7e103e1d
```
```
cd ..
```
```
mv SoapyHackRF SoapyHackRF_grc38
```
```
zip -r SoapyHackRF_grc38.zip SoapyHackRF_grc38
```
```
cd SoapyHackRF_grc38 && mkdir build && cd build
```
```
cmake ..
```
```
make
```
```
make install
```
```
ldconfig
```
```
cd ../..
```

## PLUG HACKRF AND TEST IT

```
hackrf_info
```
```
SoapySDRUtil --info
```
Available factories...hackrf, null,
```
SoapySDRUtil --probe="driver=hackrf"
```
```
SoapySDRUtil --make="driver=hackrf"
```

## Installing SoapyUHD
```
git clone https://github.com/pothosware/SoapyUHD
```
```
cd SoapyUHD/
```
```
git checkout 47972ba8b96beffb79915e300acea168bacd8d84
```
```
cd ..
```
```
mv SoapyUHD SoapyUHD_grc38
```
```
zip -r SoapyUHD_grc38.zip SoapyUHD_grc38
```
```
cd SoapyUHD_grc38 && mkdir build && cd build
```
```
cmake ..
```
```
make
```
```
make install
```
```
ldconfig
```
```
cd ../..
```

## Test uhd probe 
```
uhd_usrp_probe
```

## Installing GNURADIO
* https://wiki.gnuradio.org/index.php/UbuntuInstall  
* https://wiki.gnuradio.org/index.php?title=LinuxInstall#From_Source  
* https://github.com/gnuradio/volk/issues/340  
```
apt-get update && apt-get clean && apt-get autoremove && apt-get install -y apt-utils
```
```
apt-get install -y build-essential cmake git pkg-config python3-mako python3-numpy python3-distutils gcc-9 g++-9 gdb
```
```
git clone https://github.com/gnuradio/gnuradio
```
```
mv gnuradio gnuradio_38
```
```
cd gnuradio_38
```
```
git checkout maint-3.8  
```
git pull --recurse-submodules=on  
git submodule update --init  
```
git submodule init && git submodule update
```
```
cd ..
```
```
zip -r  gnuradio_38.zip  gnuradio_38
```
```
cd gnuradio_38 && mkdir build && cd build
```
```
cmake -DCMAKE_BUILD_TYPE=Release -DPYTHON_EXECUTABLE=/usr/bin/python3.8 ../
```
```
make 
```
```
make test
```
```
make install
```
```
ldconfig
```
``` 
export PYTHONPATH=/usr/local/lib/python3/dist-packages:/usr/local/lib/python3.8/dist-packages:$PYTHONPATH
```
```
export LD_LIBRARY_PATH=/usr/local/lib:$LD_LIBRARY_PATH
```
```
cd ../..
```

## TEST GNURADIO COMPAGNION
```
gnuradio-companion
```
## INSTALLING GR-OSMOSDR
```
git clone https://github.com/osmocom/gr-osmosdr
```
```
cd gr-osmosdr/
```
```
git checkout cffef690f29e0793cd2d6c5d028c0c929115f0ac
```
```
cd ..
```
```
mv gr-osmosdr gr-osmosdr_grc38
```
```
zip -r gr-osmosdr_grc38.zip gr-osmosdr_grc38
```
```
cd gr-osmosdr_grc38 && mkdir build && cd build
```
```
cmake ..
```
```
make
```
```
make install
```
```
ldconfig
```
```
cd ../..
```
```
cd ..
```

## RUNNING CLEVERJAM 
```
git clone https://github.com/jhonnybonny/CleverJAM
```
```
zip -r CleverJAM.zip CleverJAM/
```
```
mv CleverJAM.zip ../Desktop/ltehack_backup/
```
```
cd CleverJAM/sources
```

# RUN GNURADIO COMPANION + FILE AND OPEN jam.grc + SET CORRECT FREQUENCY
```
gnuradio-companion
```
# Monitoring Mode Frequency
USE "LTE DISCOVERY" OR "NETWORK SIGNAL GURU"   
OR USE CODE USSD : *#*#4636#*#* on ANDROID  
OR USE CODE USSD : *#0011# on SAMSUNG  
OR USE CODE USSD : *300#12345#* on I-PHONE  

Clever jam could run with hopping frequency using python script 
regards read me cleverjam for test 


# FLASHING FIRMEWARE HACKRF : FLASHING HACKRF WITH NEW FIRMWARE

```
wget https://github.com/greatscottgadgets/hackrf/releases/download/v2023.01.1/hackrf-2023.01.1.tar.xz
``` 
``` 
tar -xvf hackrf-2023.01.1.tar.xz
``` 
``` 
cd hackrf-2023.01.1/firmware-bin/
```

PRESS DFU AND RESET
``` 
hackrf_spiflash -w hackrf_one_usb.bin
``` 
PRESS RESET

SOMETIMES, DFU IS NEED  
apt-get install dfu-util  
dfu-util -D hackrf_one_usb.dfu   

# Test : plug hackrf
```
hackrf_info
```
```
SoapySDRUtil --info
```



# Documentations 
* https://github.com/SitrakaResearchAndPOC/Readme_hacklte/blob/main/hacklte_readme.txt
* https://github.com/jhonnybonny/CleverJAM
* https://www.youtube.com/watch?v=ETImDMxJr8g&pp=ygUJY2xldmVyamFt
* https://wiki.gnuradio.org/index.php?title=ModuleNotFoundError#B._Finding_the_Python_library
* https://wiki.gnuradio.org/index.php/UbuntuInstall
* https://wiki.gnuradio.org/index.php/UbuntuInstall  
* https://wiki.gnuradio.org/index.php?title=LinuxInstall#From_Source  
* https://github.com/gnuradio/volk/issues/340  
