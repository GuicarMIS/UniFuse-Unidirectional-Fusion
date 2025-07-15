# Setting Up the Repository

To run this repository, follow these steps:

## 1. Install Python and pip (on Ubuntu)

First, make sure Python and pip are installed on your system. Open a terminal in the project's root folder and run the following commands:

```bash
sudo apt update
sudo apt install python3 python3-pip
```

I have only tested the repository with Python 3.8.10 and Ubuntu 22.04. It is possible newer versions could lead to package conflicts. If that is the case, try installing specifically:

```bash
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt-get update
sudo apt-get install python3.8
```

In the case you opt for the latter, replace ``python3`` with ``python3.8`` in the following commands.

In case there are torch issues:
```
pip3 install torch==1.13 torchaudio==0.13 torchvision==0.14
```

## 2. Set up and activate virtual environment

```
sudo apt install python3.8-venv
python3 -m venv env
source env/bin/activate
```

## 3. Update pip

```
pip install --upgrade pip
```

## 4. Install requirements

```
pip install -r UniFuse/requirements.txt
```

## 5. Run the code
```
cd UniFuse/
python3 inference.py --data_path path/to/data/ --save_samples --output_path path/to/results/
```


