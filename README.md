# SRF LABEL Code Scan

A tool for extracting useful informormation for SRF.

## Installation

This will work with Ubuntu 22.04. Earlier versions might not support PaddleOCR module due to no GCC 12 support.

### Install PaddlePaddle

https://www.paddlepaddle.org.cn/documentation/docs/en/install/index_en.html

For systems with GPU / CUDA set up:
`pip install paddlepaddle-gpu==2.6.0 -i https://mirror.baidu.com/pypi/simple`

For CPU only:
`pip install paddlepaddle==2.6.0 -i https://mirror.baidu.com/pypi/simple`

Add PaddleOCR and Parseq repositories to source:
`git submodule update --recursive`

### Dependency Install

Poetry:
`poetry install --no-root`

Pip:
`pip install -r requirements.txt`

### Usage

`python main.py`


## **Poetry Installation**
Before proceeding with the latest installation, it has to be ensured that the previous installation is removed.

```
curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python3 - --uninstall

curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/install-poetry.py | python3 - --uninstall
```

Once the above is confirmed and aws login is complete, this command should be executed to install the latest poetry. 

```
curl -sSL https://install.python-poetry.org | python3 -
```

After installation, the following line should be added in bashrc and zshrc files.
```
export PATH="/home/koireader/.local/bin:$PATH"
```

Check the poetry installation using the following command:
```
poetry --version
```

Now, the install.sh should be executed in the root directory to install all the dependencies in the new conda environment using the command:
```
./scripts/install.sh
```

