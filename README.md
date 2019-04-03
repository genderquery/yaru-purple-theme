# Yaru Purple

Based on https://github.com/ubuntu/yaru/

# Building and Installing

## Using pdebuild on Debian-based distros

```sh
# clone repo
git clone https://gitlab.com/genderquery/yaru-purple-theme.git

# install build packages
sudo apt install pbuilder devscripts

# create base image
sudo pbuilder create

# build package
cd yaru-purple-theme && pdebuild -us -uc

# install built packages
sudo apt install /var/cache/pbuilder/result/yaru-theme*.deb
```