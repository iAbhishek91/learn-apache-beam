# Development environment

Instead of doing the settings on local machine its better to use some cloud platform.

Here we are using **colab**, but you can optionally use **google cloud shell**.

## Installation

- Beam supports Python-2 as of today.
- Need to install python
- Install beam "pip install -quite apache_beam[gcp]" | !{'pip install --quite apache_beam'} from python.

```sh
python3 --version
pip3 --version
sudo pip3 install -U pip
pip3 install apache-beam
```

```py
!{'python3 --version'}
!{'pip3 --version'}
!{'sudo pip3 install -U pip'}
!{'pip3 install apache-beam[gcp]'}
```
