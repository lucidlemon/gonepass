# Gonepass
Do you love 1Password? Do you also run Linux? Don't you hate that your 1Password data can't be used on Linux? Use Gonepassword!

## Building
Building gonepassword assumes you have the following things installed on your system
* Gtk+3
* Gtkmm 3.0
* Openssl
* pkg-config
* cmake >= 3.0
* a working C compiler

Gonepass uses cmake 3.0! To build, make a build directory and run cmake and then make/make install.

First make sure you have all dependencies installed.

```
sudo apt-get update
sudo apt-get install git libgtkmm-3.0-dev libssl-dev
```

Now lets start the installation

```
git clone https://github.com/jbreams/gonepass.git
cd gonepass
mkdir build
cd build
cmake ..
make
sudo make install
```

If everything went good so far, you may start the application by typing

```
/usr/local/bin/gonepass
```

## Great, now what?
When you start gonepass point it at your password vault in Dropbox. You should select the folder that ends with `agilekeychain` and type in your master password.

![alt tag](https://raw.github.com/jbreams/gonepass/gh-pages/images/gonepass_unlock.png)

If you want to load up multiple password vaults, just go to the Application menu and click `Load`, it will pop up a new window for selecting another password vault.

The window for selecting password vaults will remember the last password vault it successfully loaded.

Then just browse through your passwords!

![alt tag](https://raw.github.com/jbreams/gonepass/gh-pages/images/gonepass_main.png)

## That's pretty useful, can I update my items?
Not yet, sorry.

## Something isn't working?
Sorry about that, open an issue.
