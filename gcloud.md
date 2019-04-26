# gcloud instance quickstart

## install gcc
```bash
sudo apt-get update
sudo apt-get install gcc
```

## pyenv
[install deps](https://github.com/pyenv/pyenv/wiki/Common-build-problems):
```bash
sudo apt-get install -y make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev libncursesw5-dev xz-utils tk-dev libffi-dev liblzma-dev python-openssl git
```

Add to `.bashrc`:
```bash
cat >>~/.bashrc <<EOF
export PATH="/home/ryan/.pyenv/bin:$PATH"
$(pyenv init -)
$(pyenv virtualenv-init -)
EOF
```

Install some versions:
```bash
pyenv install 2.7.15 3.6.8 3.7.2
pyenv global 3.7.2
```


## install pip
```bash
curl "https://bootstrap.pypa.io/get-pip.py" -o "get-pip.py"
sudo python get-pip.py
pip install --upgrade pip
```

## Install jupyter
```bash
pip install jupyter
```

## other misc installs
```bash
sudo apt-get install -y htop emacs
```