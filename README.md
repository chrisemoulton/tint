#DEPRECATED: SEE http://github.com/trueinteractions/tint2#


**Official Tint - Node.js + Blink**

Tint is a runtime based on node.js, chromium (specifically blink) and node-webkit enhanced with support for creating
feature full MacOSX and Windows applications with native interfaces.  All with Javascript, HTML and CSS.  

* General Information: https://www.trueinteractions.com/
* Download: https://www.trueinteractions.com/trial.zip
* Github: https://github.com/trueinteractions/tint/
* Issues/Features: http://github.com/trueinteractions/tint/

How to Build
* Follow Chromium's Build instructions with the following exceptions:
* Instead of Google's chromium repo; use https://github.com/trueinteractions/chromium.git
* Configuring: ./build/gyp_chromium content/content.gyp to configure to build a 32-bit versoin.
* Building: ninja -C out/Release nw (or build the nw target in MSVS/XCODE).

If you have not purchased a license you'll not be able to get the sources for the compiler and SDK. Based on node-webkit, chromium (blink), v8 and other open source projects.
