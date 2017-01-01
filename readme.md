LOCAL_MANIFEST
========================

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
    $ repo init -u https://github.com/AOKP/platform_manifest.git -b nougat
    $ curl --create-dirs -L -o .repo/local_manifests/cm-14.1.xml -O -L https://raw.githubusercontent.com/MSM8916/local_manifest/aokp/cm-14.1.xml
```
### For sync: ###
```bash
    $ repo sync -j4
```
### To build for your device.. ###
```bash
    $ . build/envsetup.sh
    $ breakfast device_name_here
    $ mka bacon
```



