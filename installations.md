

## Reference Articles

* http://apple.stackexchange.com/questions/12161/os-x-terminal-must-have-utilities
* http://marcgrabanski.com/setting-up-mac-osx-web-development/
* https://miteshshah.github.io/mac/things-to-do-after-installing-mac-os-x/
* https://mattstauffer.co/blog/setting-up-a-new-os-x-development-machine-part-2-global-package-managers
* https://miteshshah.github.io/mac/install-network-tools-on-mac-os-x/

# New Computer Installation

## Brew
[Homepage](http://brew.sh/)

Install via ruby:
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Tap the versions keg:
```
brew tap homebrew/versions
```

Other Base Stuff

* GNU `find`, `locate`, `updatedb`, and `xargs`, `g`-prefixed, `sed`
  ```
  brew install coreutils moreutils findutils
  brew install homebrew/dupes/grep
  brew install homebrew/dupes/screen
  brew install gnu-sed --with-default-names
  ```

* generic [colouriser](http://kassiopeia.juls.savba.sk/~garabik/software/grc/)  
  ```
  brew install grc
  ```

* Install wget with IRI support
  ```
  brew install wget --with-iri
  ```

* Install more recent versions of some OS X tools
  ```
  brew install vim --override-system-vi
  ```

* zsh, with oh-my-zsh
  ```
  brew install zsh
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
  ```
* Updates openssh
  ```
  brew install homebrew/dupes/openssh
  ```

## Brew Cask Installation
A nice way of installing GUI packages, along with [updating them](https://github.com/buo/homebrew-cask-upgrade).

```
brew install caskroom/cask/brew-cask
brew tap caskroom/versions
brew tap buo/cask-upgrade
```

To Update Brew and Casks:

```
brew update
brew cu
brew doctor
brew cleanup
brew prune
```


## Programs

* Terminals
  ```
  brew cask install --force iterm2-beta
  ```

* Browsers
  ```
  brew cask install --force filezilla
  brew cask install --force firefox
  brew cask install --force google-chrome
  brew cask install --force waterfox
  brew cask install --force thunderbird
  ```

* Music
  ```
  brew cask install --force amazon-music
  brew cask install --force spotify
  brew cask install --force vlc
  brew cask install --force pandora
  brew cask install --force rdio
  ```

* Editors, merge tools
  ```
  brew cask install --force atom
  brew cask install --force libreoffice
  brew cask install --force microsoft-office
  brew cask install --force phpstorm textexpander textwrangler webstorm
  brew cask install --force hex
  brew cask install --force araxis-merge
  brew cask install --force sublime-text
  brew cask install --force macvim
  brew cask install --force aquamacs
  brew cask install --force skitch
  brew install doxygen
  ```

* Compression
  ```
  brew install unrar
  brew cask install the-unarchiver
  ```

* Fonts
  ```
  brew cask install --force font-noto-sans-hebrew
  brew cask install --force font-open-sans-hebrew
  brew cask install --force font-open-sans-hebrew-condensed
  ```

* Chats
  ```
  brew cask install --force telegram gitter skype slack-beta
  brew cask install --force messenger-for-desktop
  brew cask install --force adium
  ```

* Adobe
  ```
  brew cask install --force adobe-air adobe-reader
  ```

* Cloud Sync, passwords
  ```
  brew cask install --force dropbox insync
  brew cask install --force lastpass
  brew cask install --force keepassx
  ```

* Tweaks
  ```
  brew cask install --force steermouse
  ```

* Calendars
  ```
  brew cask install --force itsycal
  ```

* Uninstaller Programs
  ```
  brew cask install --force appcleaner
  ```

* Other Sweet Utils
  ```
  brew cask install --force path-finder
  brew cask install --force xquartz
  brew cask install --force burn ccleaner
  brew cask install --force ejector
  brew cask install --force mounty
  brew cask install --force flux
  brew cask install --force controlplane
  brew cask install --force disk-inventory-x
  brew cask install --force airparrot
  brew cask install --force alfred
  brew cask install --force controlplane
  brew cask install --force macid
  brew cask install --force java
  ```

* SDKs
  ```
  brew cask install --force android-studio
  brew install android-sdk
  ```

* Torrent, Downloaders
  ```
  brew cask install --force deluge
  brew cask install --force folx
  ```

* VNC
  ```
  brew cask install --force vnc-viewer
  ```

* VPN
  ```
  brew cask install --force tunnelblick
  ```

* Drawing, Multimedia, Graphics
  ```
  brew cask install --force gimp
  brew cask install --force colorpicker colorpicker-hex colorsnapper
  brew cask install --force ffmpegx
  # brew install ffmpeg
  brew install ffmpeg --with-libvpx
  brew install imagemagick --with-webp
  brew cask install --force inkscape
  brew cask install --force handbrake handbrakebatch handbrakecli
  brew cask install --force omnigraffle
  brew cask install --force id3-editor
  brew cask install --force mp3tag
  brew cask install --force kodi
  brew cask install --force sling
  ```

* Databases
  ```
  brew cask install --force navicat-premium mongochef
  brew cask install --force robomongo
  ```

* VMs
  ```
  brew cask install --force virtualbox
  brew cask install --force vmware-fusion
  brew install docker-machine
  ```

* Internet Utils
  ```
  brew cask install --force wireshark

  brew install nmap
  brew install mtr
  sudo chown root:wheel /usr/local/Cellar/mtr/0.86/sbin/mtr
  sudo chmod u+s /usr/local/Cellar/mtr/0.86/sbin/mtr
  brew install nikto
  brew install dnsmap
  ```

* Version Control
  ```
  brew install git
  brew cask install --force github-desktop
  ```

* Node, Databases
  ```
  brew install node
  brew install mongodb
  ```

* Encryption, MD5 
  ```
  brew install mcrypt
  brew install md5sha1sum
  brew install mhash
  ```


## Other programs that do not have casks
* radium
* cisco any connect
* [MagicPrefs](http://magicprefs.com/)
* [Better Touch Tool](http://blog.boastr.net/)
* [MenuMeters](http://www.ragingmenace.com/software/menumeters/)
* [Flash Player](http://get.adobe.com/flashplayer/otherversions/)
* [Java RE](http://www.oracle.com/technetwork/java/javase/downloads/index.html)
* [Silverlight](http://www.microsoft.com/getsilverlight/Get-Started/Install/Default.aspx)


## Tweaks

* steermouse

For issues with scrolling while trying to middle click:
```
  Wheel Mode: Ratchet, uncheck smooth scroll
```


* Inhibit .DS_Store and .AppleDouble from being created on network drives [Link](http://www.mac-forums.com/forums/switcher-hangout/275107-appledouble-file-directory.html)

```
defaults write com.apple.desktopservices DSDontWriteNetworkStores true
```

### Uncategorized brew apps -- things I haven't taken the time to sort

  ```
  brew install ansible
  brew install apg
  brew install apr
  brew install apr-util
  brew install arping
  brew install autossh
  brew install bdw-gc
  brew install c-ares
  brew install cairo
  brew install d-bus
  brew install dbus
  brew install dialog
  brew install expect
  brew install faac
  brew install ffind
  brew install fftw
  brew install figlet
  brew install findutils
  brew install fontconfig
  brew install freetype
  brew install gdbm
  brew install gdk-pixbuf
  brew install geoip
  brew install gettext
  brew install giflib
  brew install git
  brew install glib
  brew install gmp
  brew install gnu-sed
  brew install gnupg
  brew install gnutls
  brew install gobject-introspection
  brew install grc
  brew install grep
  brew install harfbuzz
  brew install httpd24
  brew install icu4c
  brew install imagemagick
  brew install ipcalc
  brew install jpeg
  brew install jq
  brew install lame
  brew install libav
  brew install libcroco
  brew install libexif
  brew install libffi
  brew install libgcrypt
  brew install libgpg-error
  brew install libgsf
  brew install libnet
  brew install libpng
  brew install librsvg
  brew install libtasn1
  brew install libtiff
  brew install libtool
  brew install libvpx
  brew install libxml2
  brew install libyaml
  brew install little-cms2
  brew install lynx
  brew install makedepend
  brew install minicom
  brew install mongodb
  brew install mongodb26
  brew install moreutils
  brew install mtr
  brew install nettle
  brew install nmap
  brew install node
  brew install nvm
  brew install oniguruma
  brew install openjpeg
  brew install openssh
  brew install openssl
  brew install openssl@1.1
  brew install orc
  brew install pango
  brew install pcre
  brew install perl
  brew install php-cs-fixer
  brew install php70
  brew install pixman
  brew install pkg-config
  brew install poppler
  brew install proctools
  brew install pstree
  brew install putty
  brew install py2cairo
  brew install pygobject3
  brew install python
  brew install qprint
  brew install readline
  brew install rsync
  brew install scons
  brew install shared-mime-info
  brew install signing-party
  brew install sqlformat
  brew install sqlite
  brew install ssh-copy-id
  brew install ssldump
  brew install tcping
  brew install texi2html
  brew install thefuck
  brew install unixodbc
  brew install vips
  brew install w3m
  brew install watch
  brew install watchman
  brew install webp
  brew install wget
  brew install x264
  brew install xvid
  brew install xz
  brew install yasm
  brew install zlib
  brew install zsh
  
  
  brew install ssh-copy-id
  brew install watch
  
  brew install fish
  brew install pv
  brew install rename
  brew install tree
  brew install zopfli
  ```

