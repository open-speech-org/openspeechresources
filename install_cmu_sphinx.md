# Installation of CMU Sphinx

## Ubuntu

First you need to install some OS dependencies

```bash
sudo apt update
sudo apt install -y autoconf libtool automake
sudo apt install -y bison swig
sudo apt install -y pulseaudio libpulse-dev
```

First component in the CMU Sphinx stack is Sphinx base

```
git clone https://github.com/cmusphinx/sphinxbase
cd sphinxbase
bash autogen.sh
bash configure
make
sudo make install
```

After Sphinx Train

```bash
git clone https://github.com/cmusphinx/sphinxtrain
cd sphinxtrain
bash autogen.sh
bash configure
make
sudo make install
```

Then Pocket Sphinx

```bash
git clone https://github.com/cmusphinx/pocketsphinx
cd pocketsphinx
bash autogen.sh
bash configure
make
sudo make install
```

