**Official Tint - Node.js + Blink**

Tint is a runtime based on node.js, chromium (specifically blink) and node-webkit enhanced with support for creating
feature full MacOSX and Windows applications with native interfaces.  All with Javascript, HTML and CSS.  

* General Information: https://www.trueinteractions.com/
* Download: https://www.trueinteractions.com/trial.zip
* Github: https://github.com/trueinteractions/tint/

See http://github.com/trueinteractions/tint/ for issues, features, milestones and enhancements. 

Building:
1. Follow the chromium build process line by line, BUT:
2. Use https://github.com/trueinteractions/chromium.git as the git source (instead of chromium's source)
3. Follow the directions, once you've retrieved all the code run; ./build/gyp_chromium content/content.gyp to configure.
4. Follow the directions, once you're configured to build; run ninja -C out/Release nw (or build the nw target in MSVS/XCODE).
5. Note the SDK is not included, if the build fails (it shouldn't) but if so comment out  content/nw/nw.gypi lines with ti_bindings.h (reconfigure, recompile)
6. Note the full compiler is not included (unless you've purchased support), however a sub-set to bundle execs/app's exists in: content/nw/src/tools/compiler.js

Based on node.js, chromium (blink), and node-webkit. 
