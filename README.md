# Vaulthon

Storing git credential safely in git with a self included tool might be in the biggest dream of humanity.

# Credits

All credits goes to the original AES-128 implementation by Bo Zhu in pure python, and BoppreH for the github example repository. I didn't do anything, everything goes to them. I simply wrote aproximately 20 lines of python.

# Usage

At the root of your project:

## Windows

### Powershell

```ps1
Invoke-WebRequest -OutFile vaulthon.py https://raw.githubusercontent.com/ComminQ/Vaulthon/main/vaulthon.py
ni config.json
python vaulthon.py <key>
```

## Linux

```shell
wget -O vaulthon.py https://raw.githubusercontent.com/ComminQ/Vaulthon/main/vaulthon.py
touch config.json
./vaulthon.py <key>
```

# Example

The key to execute this example is "hello", so simply run:

```shell
git clone https://github.com/ComminQ/Vaulthon.git
cd Vaulthon
python vaulthon.py hello
```