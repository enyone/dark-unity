dark-unity
==========

Modify your Unity desktop to be more healthy to your eyes

<img src="https://raw.github.com/enyone/dark-unity/master/unity-dark.png" alt="dark-unity" />

```
sudo add-apt-repository ppa:myunity/ppa
sudo add-apt-repository ppa:tista/selene
sudo add-apt-repository ppa:tiheum/equinox
sudo add-apt-repository ppa:diesch/testing
sudo apt-get update
sudo apt-get install gnome-tweak-tool selene-theme gnome-shell-theme-selene faenza-icon-theme myunity unsettings
```
Run `gnome-tweak-tool` and select `Selene` as a window and GTK theme and `Faenza-Darkest` as a icon theme.

Log off and back in to activate all changes. Without doing so some applications may look weird (wrong colors etc..)

## Firefox
* https://addons.mozilla.org/fi/firefox/addon/ft-deepdark/

### Firefox input color issue

Create file `~/.mozilla/firefox/*.default/chrome/userContent.css` and copy-paste the following:

```
input {
border: 2px inset white;
background-color: white;
color: black;
-moz-appearance: none !important;
}

textarea {
border: 2px inset white;
background-color: white;
color: black;
-moz-appearance: none !important;
}

select {
border: 2px inset white;
background-color: white;
color: black;
-moz-appearance: none !important;
}

input[type="radio"],
input[type="checkbox"] {
border: 2px inset white ! important;
background-color: white ! important;
color: ThreeDFace ! important;
-moz-appearance: none !important;
}

*|*::-moz-radio {
background-color: white;
-moz-appearance: none !important;
}

button,
input[type="reset"],
input[type="button"],
input[type="submit"] {
border: 2px outset white;
background-color: #eeeeee;
color: black;
-moz-appearance: none !important;
}

body {
background-color: white;
color: black;
display: block;
margin: 8px;
-moz-appearance: none !important;
}
```

Save-as and restart Firefox.


## Thunderbird
* https://addons.mozilla.org/en-us/thunderbird/addon/tt-deepdark/
