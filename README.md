# Flutter Crash Course

Flutter is a Google UI toolkit for building natively compiled apps for mobile, web, and desktop.

- Build iOS and Android apps using a single codebase
- Cross Platform - Mac/Windows/Linux
- Extremely Fast

## Dart Programming Language

Flutter uses and OOP language called Dart, which is optimized for UI, fast on all platforms, and similar to JS with elements of Java.

- Everything in Flutter is a widget
- Uses Material design
- Scaffold, AppBar, Container, Image, Icon, etc
- Stateless and Stateful
- Build Method

```sh
# INSTALL FLUTTER
# ...
# INSTALL DART SDK
sudo apt-get install dart; sudo apt-get update;
sudo sh -c 'wget -qO- https://storage.googleapis.com/download.dartlang.org/linux/debian/dart_stable.list > /etc/apt/sources.list.d/dart_stable.list'
sudo sh -c 'wget -qO- https://dl-ssl.google.com/linux/linux_signing_key.pub | apt-key add -'
echo 'export PATH="$PATH:/usr/lib/dart/bin"' >> ~/.profile
pub --help # "Pub is a package manager for Dart"

# CHECK FLUTTER AND DART INSTALLATION
which flutter dart # Check the location/existence of flutter and dart binaries
flutter upgrade --force
flutter doctor -v # Check installation in verbose mode
flutter sdk-path # Get the path to the Flutter SDK
flutter devices # List devices available through Android Device Bridge
flutter emulators # List available emulators
flutter emulators --launch Pixel_3a_API_30_x86

# SETUP HARDWARE ACCELERATION
sudo apt-get install cpu-checker
egrep -c '(vmx|svm)' /proc/cpuinfo
kvm-ok
sudo apt-get install qemu-kvm libvirt-daemon-system libvirt-clients bridge-utils
sudo adduser (id -un) libvirtd
virsh list --all

```

## VS Code Setup

- Install Flutter extension
- Install Dart extension
View > Flutter: Run Flutter Doctor
View > Flutter: Run Flutter Upgrade
View > Flutter: New Project
