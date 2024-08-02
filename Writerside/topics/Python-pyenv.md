# Python - pyenv

Install Python build dependencies [https://github.com/pyenv/pyenv/wiki#suggested-build-environment](https://github.com/pyenv/pyenv/wiki#suggested-build-environment)

**Ubuntu/Debian/Mint:**

```bash
sudo apt update; sudo apt install build-essential libssl-dev zlib1g-dev \
libbz2-dev libreadline-dev libsqlite3-dev curl git \
libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
```

pyenv installer [https://github.com/pyenv/pyenv-installer](https://github.com/pyenv/pyenv-installer)

```bash
curl https://pyenv.run | bash
```



```bash
export PYENV_ROOT="$HOME/.pyenv"
[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init -)"
```



## 3.10.14

```bash
mkdir ~/.pyenv/cache -p

cd ~/.pyenv/cache

wget https://mirrors.huaweicloud.com/python/3.10.14/Python-3.10.14.tar.xz

pyenv install 3.10.14

pyenv global 3.10.14
```

pip 全局配置清华大学镜像

```bash
pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
pip config set install.trusted-host pypi.tuna.tsinghua.edu.cn
```

pip 全局配置文件路径： **~/.config/pip/pip.conf**
