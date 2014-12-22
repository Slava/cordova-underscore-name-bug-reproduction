Bug reproduction in Cordova
===

When a folder name starts with '_' (underscore), the file is not served.

In this reproduction you can see it is the default Cordova app with folder
www/css moved to www/_css. The reference to Css files in index.html was also
fixed to _css/index.css.

Run the app with `cordova run android --emulator` and observe that the
stylesheet is missing.

