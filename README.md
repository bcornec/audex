Audex
=====

Audex is an audio grabber tool for CD-ROM drives for the KDE desktop.

### Prerequisites

* libkcddb
* libkcompactdisc
* cdparanoia

### Prerequisites (optional)

* Ogg Vorbis (ogg files)
* FLAC (flac files)
* LAME (mp3 files)
* FAAC (mp4/aac files)
* eyeD3 (mp3 tagging)

### Compile

mkdir build
cd build
cmake -DCMAKE_VERBOSE_MAKEFILE=ON -DCMAKE_BUILD_TYPE=Debug -DCMAKE_INSTALL_PREFIX=/usr ..
make
(sudo) make install

### Further information

These files make Audex linux dependant:

* utils/pid.h
* utils/pid.cpp

These files make Audex cdda paranoia dependant:

* utils/cddaparanoia.h
* utils/cddaparanoia.cpp

### KF5 Port TODO

* Port KMimeType::defaultMimeType() (to QMimeType::isDefault()?)
* Port KDialog
* Port KLineEdit
* Check KIO job->
* Check KUrl
* Use solid instead of libkcompactdisc?

