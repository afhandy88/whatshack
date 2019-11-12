# whatshack
Install dependencies:
# apt-get update
# apt-get install openjdk-8-jdk
# apt-get install gradle

Use Java8:
Get Java8 dir with command:
# update-alternatives --list java

Copy and replace dir on command:
# update-alternatives --set java /usr/lib/jvm/java-8-openjdk-amd64/jre/bin/java

Download Android Studio:
https://developer.android.com/studio

Installing Android Studio:
# unzip ~/Downloads/android*.zip -d /opt

For AMD64 Arch, Install Android Studio dependencies:
# apt-get install lib32z1 lib32ncurses6 lib32stdc++6


Run Android Studio:
# cd /opt/android-studio/bin
# ./studio.sh

Go to SDK Manager (Configure -> SDK Manager) and Download:
Android SDK Build-tools, Android SDK-tools, Android SDK platform-tools, Support Repository

Run script:
# git clone https://github.com/thelinuxchoice/whatshack
# cd whatshack/
# bash whatshack.sh


On First Time, Choose "n" when asks to build, then open the project on Android Studio:
cd /opt/android-studio/bin
./studio.sh

Import Gradle Project:
Choose whatshack app folder: whatshack/app/

Wait all dependencies downloading, if you got errors, click on showed links to solve.
Try build from Android Studio: Build > build APK's
Click on showed links if you got errors.
Close Android after building successfully.

open with any Text Editor the file app/build.gradle

remove "google()"
change gradle version from: 3.4.1 to: 2.2.0
save and exit.

Run script (as root):
# bash whatshack.s
