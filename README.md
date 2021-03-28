# PiShrink
Backup and shrink your raspberry pi os directly from sd card.

## Installation
```
wget https://raw.githubusercontent.com/ammababoi/PiShrink/main/pishrink && sudo chmod +x pishrink && sudo cp pishrink /usr/bin/ && sudo apt install pv -y
```
## Usage

Know your device name
```
df -h
```
now extract the device name

example 1 for list entries like:

/dev/sda1 + /dev/sda2

remove digit at the end

result:

/dev/sda

example 2 for list entries like:

/dev/nvme0n1p6 + /dev/nvme0n1p1

remove p and digit at the end

result:

/dev/nvme0n1

Run command

```
sudo pishrink device /dev/{your sd card name}
```

## Example
```
sudo pishrink device /dev/sda
```

## This repository was inspired from

[pishrink](https://github.com/Drewsif/PiShrink) and [shrink](https://github.com/qrti/shrink)
