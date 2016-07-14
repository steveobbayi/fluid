Fluid
=====

[![ZenHub.io](https://img.shields.io/badge/supercharged%20by-zenhub.io-blue.svg)](https://zenhub.io)

[![License](https://img.shields.io/badge/license-LGPLv2.1%2B-blue.svg)](http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html)
[![GitHub release](https://img.shields.io/github/release/qmlos/fluid.svg)](https://github.com/qmlos/fluid)
[![Build Status](https://travis-ci.org/qmlos/fluid.svg?branch=develop)](https://travis-ci.org/qmlos/fluid)
[![GitHub issues](https://img.shields.io/github/issues/qmlos/fluid.svg)](https://github.com/qmlos/fluid/issues)
[![Maintained](https://img.shields.io/maintenance/yes/2016.svg)](https://github.com/qmlos/fluid/commits/develop)

Fluid is a collection of cross-platform QtQuick components for building fluid and dynamic applications.

### Dependencies

Qt >= 5.7.0 with at least the following modules is required:

* [qtbase](http://code.qt.io/cgit/qt/qtbase.git)
* [qtdeclarative](http://code.qt.io/cgit/qt/qtdeclarative.git)
* [qtquickcontrols](http://code.qt.io/cgit/qt/qtquickcontrols.git)
* [qtquickcontrols2](http://code.qt.io/cgit/qt/qtquickcontrols2.git)
* [qtgraphicaleffects](http://code.qt.io/cgit/qt/qtgraphicaleffects.git)

### Installation

First, if you want to include the Material Design icons used with the `Icon` component, run:

```sh
./scripts/fetch_icons.sh
```

This will clone the Google repository holding the icons and copy the SVG icons into the `icons` directory.

From the root of the repository, run:

```sh
mkdir build; cd build
cmake .. -DKDE_INSTALL_USE_QT_SYS_PATHS=ON
make
make install # use sudo if necessary
```

On the `cmake` line, you can specify additional configuration parameters:

 * `-DCMAKE_INSTALL_PREFIX=/path/to/install` (for example, `/opt/qmlos` or `/usr`)
 * `-DCMAKE_BUILD_TYPE=<build_type>`, where `<build_type>` is one of:
   * **Debug:** debug build
   * **Release:** release build
   * **RelWithDebInfo:** release build with debugging information

### Licensing

Fluid is free software; you can redistribute it and/or
modify it under the terms of the GNU Lesser General Public
License as published by the Free Software Foundation; either
version 2.1 of the License, or (at your option) any later version.
