[![Build Status](https://travis-ci.org/openpst/openpst.svg?branch=master)](https://travis-ci.org/openpst/openpst)

# OpenPST

OpenPST is currently in early development.

###Goals
OpenPST aims to be a multi-platform phone servicing tool for Qualcomm based chipsets.

###Dependencies

 - [QT 5.x](https://www.qt.io/download/)
 - [Serial library by wjwwood](http://wjwwood.github.com/serial/)

### Building

    git clone https://github.com/openpst/openpst --depth=1
    cd openpst
    git submodule init
    git submodule update --depth=1

####Windows

 1. Install QT
 2. Install QT Visual Studio plugin
 3. Setup QT enviornment in Visual Studio
 4. Open `OpenPST-vs2013.sln` in root of project
 5. Build

#### Linux

 1. Install build essentials and QT libraries
 2. Run `make` from root of project

#### QT Creator

 1. Open OpenPST.pro in QT Creator. Build

### Currently Worked On Features
- Sahara Protocol
	- Image Transfer
	- Client Commands
	- Memory Debug/Read

- Streaming DLOAD Protocol
	- General features
	- Read flash
	- Open image / read & write
	- Open multi / read & write

- QCDM
	- General NAM programming
	- NV Read/Write
	- Memory Read
	
- MBN Inspection
	- Quickly view header for 80 byte and 40 byte variants
	- Identify image type
	- Identify OEM_ID, MODEL_ID, etc
	- Extract real image, signature, and certificate
	
- ADB Partition Backup and Inspection Utilities
	- Create partition xml from working devices
	- Backup partitions from working devices
