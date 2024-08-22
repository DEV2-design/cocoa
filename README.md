# Qt cocoa plugin

Cocoa is a native application development framework for the macOS platform, providing a rich set of APIs for desktop application development. In the macOS port of Qt, Cocoa is used as a plugin module.
Within the Qt environment, Cocoa is integrated as a module, allowing developers to invoke macOS native features within their Qt projects.
The Qt port of cocoa currently compiles and runs on macOS.

# Building

You can build and install cocoa plugin with these commands:

# Qt5.6.3 (base on macOS10.10 and macosx10.11)
cd /Users/imyfone/Qt5.6.3/5.6.3/Src/qtbase
./configure -sdk macosx10.11 -no-sql-psql -prefix /Users/imyfone/Qt5.6.3/5.6.3/clang_64 -opensource -confirm-license -debug-and-release -separate-debug-info -nomake examples -nomake tests -force-debug-info -strip
make && make install

# Qt5.15.2 (base on macOS10.13 and macosx 10.14)
cd /Users/mf2019/Qt/5.15.2/Src/qtbase
./configure -sdk macosx10.14 -no-sql-psql -prefix /Users/mf2019/Qt/5.15.2/clang_64 -opensource -confirm-license -debug-and-release -separate-debug-info -nomake examples -nomake tests -force-debug-info -strip
make && make install

See https://github.com/qt/qtbase/blob/dev/cmake/README.md for more detailed instuctions
