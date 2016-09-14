LOCAL_MANIFEST
========================
CM-14.0 for Moto G 2015  (OSPREY)

### Installing Repo ###
```bash
# Make a directory where Repo will be stored and add it to the path
    $ mkdir ~/.bin
    $ PATH=~/.bin:$PATH

# Download Repo itself
    $ curl https://storage.googleapis.com/git-repo-downloads/repo > ~/.bin/repo

# Make Repo executable
    $ chmod a+x ~/.bin/repo
```

### Initializing Repo ###
```bash
    $ repo init -u https://github.com/CyanogenMod/android.git -b staging/cm-14.0
    $ curl --create-dirs -L -o .repo/local_manifest/cm-14.0.xml -O -L https://raw.githubusercontent.com/OSPREY-N/local_manifest/cm-14.0/cm-14.0.xml
```
### For sync: ###
```bash
    $ repo sync -j4
```
### To build for your device.. ###
```bash
    $ build/envsetup.sh
    $ brunch device_name_here
```



