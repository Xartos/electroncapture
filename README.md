This is the **Electron Capture app**, created for <a href="https://obs.ninja">OBS.Ninja</a> users. It's designed to allow for easy "Screen Capturing" of OBS.Ninja live video streams using applications like OBS. 

<a href="https://github.com/steveseguin/electroncapture#links-to-downloads-below">Jump to Downloads Section</a>

<img src="https://user-images.githubusercontent.com/2575698/80891745-290d3000-8c94-11ea-85c4-ae0e7cd1ec19.png " alt="" data-canonical-src="https://user-images.githubusercontent.com/2575698/80891745-290d3000-8c94-11ea-85c4-ae0e7cd1ec19.png "  height="300" />

## Why ?
OBS on macOS currently doesn't support its Browser Source plugin all that well, so this tool is a viable alternative. It lets you cleanly screen-grab just a video stream without the need of the Browser Source plugin. It also makes it easy to select the output audio playback device, such as a Virtual Audio device: ie) https://rogueamoeba.com/audiohijack/

The app also remains on top of other windows, attempts to hide the mouse cursor when possible, and provides accurate window sizes for 1:1 pixel mapping.

Windows users may find it beneficial too, as it offers support for OBS.Ninja's &buffer audio sync command and it has robust support for video packet loss. In other words, it can playback live video better than OBS can, with fewer video playback errors and better audio/video sync. If you have a spare monitor, it may at times be worth the hassle to use.



## Settings and Parameters

The default frameless resolution of the capture window is 1280x720. The app automatically accounts for high-DPI displays, so it is always 1:1 pixel-accurate with the specified resolution on even Apple Retina displays.

The optional Command Line arguments can be seen as examples below, along with their default values.

```
OBSN.exe --width 1280 --height 720 --url https://obs.ninja/electron
```
or for example
```
./OBSN -w 1280 -h 720 -u https://obs.ninja/electron
```

## Notes on Using and Closing the App

For Windows users, right click to bring up the context menu, which allows you to close the app. You can also press ALT-F4 in many cases.

For Mac users, you can hover your mouse cursor over the top-left corner of the app to show the close button.

Also note, the top portion of the app is draggable, so you can move it around to place it accordingly. It is also resizable.

Multiple versions of the app can run on macOS; just make a copy of the file with a different name to open up a new window.

# Links to downloads below.

You can find the newest release builds of the app here: https://github.com/steveseguin/electroncapture/releases  or see below.

### Windows Version
- Installs the app for easy loading from Start Menu
https://github.com/steveseguin/electroncapture/releases/download/1.05/electron_win_installer.zip

- Portable version; no install needed
https://github.com/steveseguin/electroncapture/releases/download/1.05/electron_win_portable.zip 

### Mac Version
https://github.com/steveseguin/electroncapture/releases/download/1.05/obs-ninja-da-1.0.5.dmg 

### Linux Version
(likely best to build it yourself?)


## Building the App from Source

You'll need to download and extract the source code; or git clone it.
You'll also need npm installed.

### To run the app from source, you can:
```
npm install
npm start
```

### Building the app from source:
Building does not support cross-compiling. In order to build you must be logged in to a host having the target OS for the build. Once logged in, type the following:

```
npm install
npm run build
```

* For Mac, please also see this issue for building: https://github.com/electron-userland/electron-builder/issues/3828

And for notorization on macOS,..
```
npm install
export appleId={yourApp@dev.email}
export appleIdPassword={app-specific-password-here}
sudo -E npm run build

```


"Electron capture is one process that unstable atoms can use to become more stable. " - https://education.jlab.org/glossary/electroncapture.html



