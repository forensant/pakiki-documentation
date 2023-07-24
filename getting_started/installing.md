# Installing/Running

## Linux

Pākiki Proxy has been tested on Kali Linux, while it should run elsewhere there may be bugs. If you run into bugs on other common distributions, feel free to report these to support@pakikiproxy.com 

### Kali and Debian, Ubuntu, etc

Download the .deb installer for your platform from your Pākiki Proxy [accounts page](https://pakikiproxy.com/pages/account) (for the Professional version) otherwise from the [downloads page](https://pakikiproxy.com/pages/downloads) for the Community version. If you are installing it onto a virtual machine on an M1 or M2 Mac, then choose arm64, otherwise x64 is generally the correct architecture.

Then to install it, run the following commands:

```bash
# update the system
sudo apt update
sudo apt upgrade

# install the package
sudo dpkg -i PakikiProxy-*.deb

# install any missing dependencies
sudo apt install -f

# optional but recommended - for the embedded browser support
sudo apt install chromium
```

The installer should create a link in the relevant application menu, however if you cannot find it, you can manually launch Pākiki Proxy with `pakiki` or `pakikipro` depending on the verison you have downloaded.

### Other distributions

Pākiki is also distributed in Flatpak format for other distributions. Flatpak is used to ensure that all dependencies are met.

To install it, first you’ll need to install Flatpak for your distribution. Instructions on how to do this for specific distributions are on the [Flatpak Website](https://flatpak.org/setup/).

After that, download the .flatpak package for your platform from your Pākiki Proxy [accounts page](https://pakikiproxy.com/pages/account) (for the Professional version) otherwise from the [downloads page](https://pakikiproxy.com/pages/downloads) for the Community version. If you are installing it onto a virtual machine on an M1 or M2 Mac, then choose arm64, otherwise x64 is generally the correct architecture. Note that for Flatpak, due to development resources, arm64 may not always be well tested and offered. Please contact [support@pakikiproxy.com](mailto:support@pakikiproxy.com) if you do require it.

Once the Flatpak package has been downloaded, it can be installed with: `flatpak install PakikiProxy-*.flatpak`

The installer should create a link in the relevant application menu, however if you cannot find it, you can manually launch Pākiki Proxy with `flatpak run com.forensant.pakiki` or `flatpak run com.forensant.pakiki-pro` depending on the version you downloaded.

## MacOS

Open the DMG file and drag Pākiki Proxy into the Applications folder to install it. It can then be run from the Applications folder, via Spotlight, etc.

 > If you like to navigate around applications with the keyboard, it is recommended that you enable `Keyboard Navigation` within your system settings. Without this enabled, you will not be able to fully navigate the Pākiki user interface with the keyboard.

## Web Interface/Forward Deployments

When the Pākiki Core is run, a web interface is also launched. By default, this listens on [http://127.0.0.1:10101](http://127.0.0.1:10101).

The web interface does not contain the same amount of functionality as the desktop applications, and is intended for forward deployments or where you needed core proxying functionality in more limited environments.

Prebuilt packages of the core are not currently available, however instructions to build/run this are available within the [GitHub repository](https://github.com/forensant/pakiki-core). Prebuilt versions may be available on request by contacting [support@pakikiproxy.com](mailto:support@pakikiproxy.com).