# Setting up Flutter: MacOS

Download the [Flutter SDK](https://docs.flutter.dev/get-started/install/macos)

Unzip it in a folder of your choice. For example...
```
cd ~/development
unzip ~/Downloads/flutter_macos_2.8.1-stable.zip
```

Add flutter as a PATH variable `echo export PATH="$PATH:[PATH_OF_FLUTTER_GIT_DIRECTORY]/bin" >> ~/.bash_profile`

Test with `flutter doctor`

In order to resolve the issues that were brought up, I needed to do the following:

* In Android Studio, go to Preferences > Appearance and Behavior > System Settings > Android SDK

* Check the box next to "Android SDK Command-line Tools (latest)" and then click Apply and follow the steps.

* run `flutter doctor --android-licenses`

* run `sudo gem install cocoapods`

* test that everything was installed by re-running `flutter doctor`!

Now you just need to decide... Material or Cupertino??