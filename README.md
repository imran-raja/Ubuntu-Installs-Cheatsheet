## A cheat-sheet of Terminal commands for installing programs after a fresh Ubuntu set-up 

* [Application](#application)

	* [Chat Clients](#chat-clients)
	* [Development](#development)
	* [Data Recovery](#data-recovery)
	* [File Managers](#file-managers)
	* [Windows on Linux](#windows-on-linux)
	* [Utilities](#utilities)
	* [Internet](#internet)
	* [File Sharing](#file-sharing)
	* [Productivity](#productivity)
	* [Pdf reader](#[pdf-reader)
	* [Audio and Video](#audio-and-video)
	* [Graphics](#graphics)


### Chat Clients
**Slack**		

> Couldn't find a Terminal command. So just download from the [official Slack download webpage](https://slack.com/downloads/linux)

**Skype**	

> Couldn't find a Terminal command. So just download from the [official Skype download webpage](https://www.skype.com/en/download-skype/skype-for-computer/)
		

### Development
**Pycharm Community Version**		

```
sudo add-apt-repository ppa:mystic-mirage/pycharm
sudo apt-get update
```		
		
**Sublime Text**	
```
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
sudo apt-get update
sudo apt-get install sublime-text
```

**CodeBlocks**
```
sudo add-apt-repository ppa:damien-moore/codeblocks-stable
sudo apt update
sudo apt install codeblocks codeblocks-contrib
```

**Octave**	
```
sudo apt-add-repository ppa:octave/stable
sudo apt-get update
sudo apt-get install octave
```

**R
```
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E298A3A825C0D65DFD57CBB651716619E084DAB9
sudo add-apt-repository 'deb [arch=amd64,i386] https://cran.rstudio.com/bin/linux/ubuntu xenial/'
sudo apt-get update
sudo apt-get install r-base
```
### Data Recovery

**TestDisk 
```
sudo apt-get update
sudo apt-get install testdisk
```

### File Managers

**Nautilus
```
sudo apt-get update
sudo apt-get install nautilus
```
### Windows on Linux

**Wine**
```
sudo dpkg --add-architecture i386
sudo apt-add-repository 'https://dl.winehq.org/wine-builds/ubuntu/'
wget https://dl.winehq.org/wine-builds/Release.key && sudo apt-key add Release.key
sudo apt update && sudo apt install winehq-stable
```	
### Utilities
**Media Codec**		
```
sudo apt install ubuntu-restricted-extras
sudo apt install libavcodec-extra
```		

**Avro**	
```
sudo apt install gjs gir1.2-ibus-1.0 libibus-1.0-5 libibus-1.0-dev ibus-gtk ibus-gtk3 ibus-clutter ibus-qt4
wget "https://github.com/maateen/avro/releases/download/v2.1/avro_2.1-3_all.deb"
sudo dpkg -i avro_2.1-3_all.deb
```	

**TLP - Linux Advanced Power Management Tool
```
sudo add-apt-repository ppa:linrunner/tlp
sudo apt-get update
sudo apt-get install tlp tlp-rdw
```
**GParted
```
sudo apt-get install gparted
```
**BleachBit
> Couldn't find a Terminal command. So just download from the [official Bleach Bit download webpage](https://www.bleachbit.org/download/linux)

**KeePassX
```
sudo add-apt-repository ppa:eugenesan/ppa
sudo apt-get update
sudo apt-get install keepassx
```

**System Load Indicator
```
sudo add-apt-repository ppa:indicator-multiload/stable-daily
sudo apt-get update && sudo apt-get install indicator-multiload
```

**Bazel**
```
sudo apt-get install openjdk-8-jdk
echo "deb [arch=amd64] http://storage.googleapis.com/bazel-apt stable jdk1.8" | sudo tee /etc/apt/sources.list.d/bazel.list
curl https://bazel.build/bazel-release.pub.gpg | sudo apt-key add -
sudo apt-get update && sudo apt-get install bazel
sudo apt-get upgrade bazel
```
### Internet

**Chromium Browser**		
```
sudo apt-get update
sudo apt-get install chromium-browser
```
### File Sharing
**Dropbox**		
```
cd ~ && wget -O - "https://www.dropbox.com/download?plat=lnx.x86_64" | tar xzf -
~/.dropbox-dist/dropboxd
```		
		
**TeamViewer
> Couldn't find a Terminal command. So just download from the [official TeamViewer download webpage](https://www.teamviewer.com/en/download/linux/)


**Go For It
```
sudo add-apt-repository ppa:go-for-it-team/go-for-it-daily && sudo apt-get update
sudo apt-get install go-for-it
```

**GNOME Dictionary	
```
apt-get install gnome-dictionary
```

### Pdf reader

**Okular**	
```
sudo apt-get update
sudo apt-get install okular
```

### Audio and Video
**VLC**		
```
sudo add-apt-repository ppa:videolan/stable-daily
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install vlc
```

**Audacity
```
sudo add-apt-repository ppa:ubuntuhandbook1/audacity
sudo apt update
sudo apt install audacity
```

### Graphics

**Inkscape
```
sudo snap remove inkscape
sudo add-apt-repository ppa:inkscape.dev/stable
sudo apt update
sudo apt install inkscape
```

