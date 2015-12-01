## sddm-theme-deepspace

It is based on the elarun theme, but really modivied!

Layout and lots more.

For example, no successfully logged in lastUser is displayed, because of security reasons.

There is no chance to activate/deactivate it via /etc/sddm.conf, i tested it and it dosen't work.

so you have to manually edit the Main.qml, because of a bug
found here: 

https://bugzilla.redhat.com/show_bug.cgi?id=1238889

So take a look to the Main.qml and read the comments!

### You want it, you get it, the Screenshot

![sample screenshot](https://raw.githubusercontent.com/siduction/sddm-theme-deepspace/master/artwork/png/preview.jpg)

### How to test

(as user) sddm-greeter --test-mode --theme ~/downloads/directory/`<theme>`/

### How to install

(as root) copy the `<theme>` to /usr/share/sddm/themes/

Be shure that the directory 'new theme' is set to drwxr-xr-x

If not, run chmod 755 'new theme'!

Otherwise you have no luck to use it!

### Needed stuff ###

Be shure you have qml-module-qtquick-controls and qml-module-qtgraphicaleffects installed!