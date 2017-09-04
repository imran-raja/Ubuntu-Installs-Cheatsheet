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
	* [pdf Readers](#pdf-readers)
	* [Audio and Video](#audio-and-video)
	* [Graphics](#graphics)


## Chat Clients
**1. Slack**		

> Couldn't find a Terminal command. So just download from the [official Slack download webpage](https://slack.com/downloads/linux)

**2. Skype**	

> Couldn't find a Terminal command. So just download from the [official Skype download webpage](https://www.skype.com/en/download-skype/skype-for-computer/)


## Development
**1. Pycharm Community Version**		

```
sudo add-apt-repository ppa:mystic-mirage/pycharm
sudo apt-get update
```		
		
**2. Sublime Text**	
```
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
sudo apt-get update
sudo apt-get install sublime-text
```

**3. CodeBlocks**
```
sudo add-apt-repository ppa:damien-moore/codeblocks-stable
sudo apt update
sudo apt install codeblocks codeblocks-contrib
```

**4. Octave**	
```
sudo apt-add-repository ppa:octave/stable
sudo apt-get update
sudo apt-get install octave
```

**5. R**
```
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E298A3A825C0D65DFD57CBB651716619E084DAB9
sudo add-apt-repository 'deb [arch=amd64,i386] https://cran.rstudio.com/bin/linux/ubuntu xenial/'
sudo apt-get update
sudo apt-get install r-base
```
## Data Recovery

**1. TestDisk**
```
sudo apt-get update
sudo apt-get install testdisk
```

## File Managers

**1. Nautilus**
```
sudo apt-get update
sudo apt-get install nautilus
```
## Windows on Linux

**1. Wine**
```
sudo dpkg --add-architecture i386
sudo apt-add-repository 'https://dl.winehq.org/wine-builds/ubuntu/'
wget https://dl.winehq.org/wine-builds/Release.key && sudo apt-key add Release.key
sudo apt update && sudo apt install winehq-stable
```	
## Utilities

**1. Media Codec**		
```
sudo apt install ubuntu-restricted-extras
sudo apt install libavcodec-extra
```		

**2. Avro**	
```
sudo apt install gjs gir1.2-ibus-1.0 libibus-1.0-5 libibus-1.0-dev ibus-gtk ibus-gtk3 ibus-clutter ibus-qt4
wget "https://github.com/maateen/avro/releases/download/v2.1/avro_2.1-3_all.deb"
sudo dpkg -i avro_2.1-3_all.deb
```	

**3. TLP - Linux Advanced Power Management Tool**
```
sudo add-apt-repository ppa:linrunner/tlp
sudo apt-get update
sudo apt-get install tlp tlp-rdw
```

**4. GParted**
```
sudo apt-get install gparted
```

**5. BleachBit**
> Couldn't find a Terminal command. So just download from the [official Bleach Bit download webpage](https://www.bleachbit.org/download/linux)

**6. KeePassX**
```
sudo add-apt-repository ppa:eugenesan/ppa
sudo apt-get update
sudo apt-get install keepassx
```

**7. System Load Indicator**
```
sudo add-apt-repository ppa:indicator-multiload/stable-daily
sudo apt-get update && sudo apt-get install indicator-multiload
```

**8. Bazel**
```
sudo apt-get install openjdk-8-jdk
echo "deb [arch=amd64] http://storage.googleapis.com/bazel-apt stable jdk1.8" | sudo tee /etc/apt/sources.list.d/bazel.list
curl https://bazel.build/bazel-release.pub.gpg | sudo apt-key add -
sudo apt-get update && sudo apt-get install bazel
sudo apt-get upgrade bazel
```
## Internet

**1. Chromium Browser**		
```
sudo apt-get update
sudo apt-get install chromium-browser
```
## File Sharing

**1. Dropbox**		
```
cd ~ && wget -O - "https://www.dropbox.com/download?plat=lnx.x86_64" | tar xzf -
~/.dropbox-dist/dropboxd
```		
		
**2. TeamViewer**
> Couldn't find a Terminal command. So just download from the [official TeamViewer download webpage](https://www.teamviewer.com/en/download/linux/)

## Productivity

**1. Go For It**
```
sudo add-apt-repository ppa:go-for-it-team/go-for-it-daily && sudo apt-get update
sudo apt-get install go-for-it
```

**2. GNOME Dictionary	
```
apt-get install gnome-dictionary
```

### pdf Readers

**1. Okular**	
```
sudo apt-get update
sudo apt-get install okular
```

## Audio and Video
**1. VLC**		
```
sudo add-apt-repository ppa:videolan/stable-daily
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install vlc
```

**2. Audacity**
```
sudo add-apt-repository ppa:ubuntuhandbook1/audacity
sudo apt update
sudo apt install audacity
```

## Graphics

**1. Inkscape**
```
sudo snap remove inkscape
sudo add-apt-repository ppa:inkscape.dev/stable
sudo apt update
sudo apt install inkscape
```

