When doing Android Open Source Project build on Linux machine, do not forget to check and / or change your `JAVA_HOME` and `PATH` environment variables to OpenJDK version -- `alternatives` command changes are not enough.  

To be precise, you need to change only `JAVA_HOME` variable using `export` command or in your init script like `~/.bash_profile`. Then `source build/envsetup.sh && lunch` command inserts `JAVA_HOME` to the begining of `PATH`.  

If you fail to do so, you will spend 2 hours trying to overcome some very strange build errors and will get nothing as a result. Do not try to `make clean` your sandbox directory as it does not help, new `repo sync` is needed.  

On information from Sony AOSP Oreo 8.0 page [https://developer.sonymobile.com/open-devices/aosp-build-instructions/how-to-build-aosp-oreo-for-unlocked-xperia-devices/](https://developer.sonymobile.com/open-devices/aosp-build-instructions/how-to-build-aosp-oreo-for-unlocked-xperia-devices/).