![Etar Calendar](./assets/_pre_prod/Feature Graphic.png)
#Etar Calendar
Etar ( From Arabic:  `إِيتَار`)  is an opensource material designed calendar made for everyone!

[![](./assets/_pre_prod/en_google_play.png)](https://play.google.com/store/apps/details?id=ws.xsoh.etar)

![Etar Calendar](./assets/_pre_prod/publish/v1.0/animation.gif)

##Why?
Well, I wanted a simple, material designed and state of the art opensoure calendar that anyone can make it more better.

###Spcical Thanks

The application is enhanced version of AOSP Calendar. Without the help of
[Free Software for Android](https://github.com/Free-Software-for-Android/Standalone-Calendar) team, 
this app well be just dream. So thanks to them!

##Features
- Month view.
- Week, day & agenda view.
- Uses Android calendar sync. Works with Google Calendar, Exchange..etc.
- Material designed.
- Agenda widget.

#### Translations in Google Play app description
You can update/add your own language [here](./assets/_pre_prod/publish/v1.0/features/). Also all artwork files are available [here](./assets/_pre_prod/)

### Build instructions
```
git submodule init
git submodule update

gradle build
```

### How this was done
- see ``build.gradle`` and the modifications to ``AndroidManifest.xml``
- ``fix_strings_and_import.py`` was created to fix a build problem and rename imports of R.java
- get time zone data from http://www.iana.org/time-zones write ``backward`` and ``zone.tab`` to assets and to assets of https://github.com/dschuermann/standalone-calendar-timezonepicker
- comment out code in https://github.com/dschuermann/standalone-calendar-frameworks-ex
