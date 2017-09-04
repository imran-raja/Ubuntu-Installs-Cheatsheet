# A cheat-sheet of Terminal commands for installing programs after a fresh Ubuntu set-up 

**1.Slack**		

> https://slack.com/downloads/linux
		
**2. Pycharm Community Version**		

```
sudo add-apt-repository ppa:mystic-mirage/pycharm
sudo apt-get update
```		
		
**3. Sublime Text**	

> wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
> echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
> sudo apt-get update
> sudo apt-get install sublime-text
		
**4. Chromium Browser**		

> sudo apt-get update
> sudo apt-get install chromium-browser
		
**5. Dropbox**		

cd ~ && wget -O - "https://www.dropbox.com/download?plat=lnx.x86_64" | tar xzf -
~/.dropbox-dist/dropboxd
		
		
**6. Octave**	

sudo apt-add-repository ppa:octave/stable
sudo apt-get update
sudo apt-get install octave
		
**7. Media Codec**		

sudo apt install ubuntu-restricted-extras
sudo apt install libavcodec-extra
		
**8. Skype**	

https://www.skype.com/en/download-skype/skype-for-computer/
		
**9. Avro**	

sudo apt install gjs gir1.2-ibus-1.0 libibus-1.0-5 libibus-1.0-dev ibus-gtk ibus-gtk3 ibus-clutter ibus-qt4
wget "https://github.com/maateen/avro/releases/download/v2.1/avro_2.1-3_all.deb"
sudo dpkg -i avro_2.1-3_all.deb
		
**10. Wine**

sudo dpkg --add-architecture i386
sudo apt-add-repository 'https://dl.winehq.org/wine-builds/ubuntu/'
wget https://dl.winehq.org/wine-builds/Release.key && sudo apt-key add Release.key
sudo apt update && sudo apt install winehq-stable
		
**11. VLC**		

sudo add-apt-repository ppa:videolan/stable-daily
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install vlc
		
**12. Okular**	

sudo apt-get update
sudo apt-get install okular

**13. Bazel**

sudo apt-get install openjdk-8-jdk
echo "deb [arch=amd64] http://storage.googleapis.com/bazel-apt stable jdk1.8" | sudo tee /etc/apt/sources.list.d/bazel.list
curl https://bazel.build/bazel-release.pub.gpg | sudo apt-key add -
sudo apt-get update && sudo apt-get install bazel
sudo apt-get upgrade bazel

