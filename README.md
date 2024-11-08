# Viriback to MISP

This project aims to get the detection generated for the project [C2 Tracker](https://tracker.viriback.com/), and create events in MISP. 

The events will be distributed by month/year and malware family, like the example below. In each event will be created objects for each IOC detected in the C2 Tracker.


|![](https://github.com/santiag02/viriback2misp/blob/main/media/misp.png)|
|:---:|
|MISP Events|

## How install

```bash
pip install viriback2misp
```

## Commands

```bash
viriback2misp -h
usage: viriback2misp [-h] [-i] [-u] [-d {0,1,2,3,4}]

Viriback C2 data to MISP events

options:
  -h, --help            show this help message and exit
  -i, --init            First step. Pass your API key and URL.
  -u, --update          Update MISP events.
  -d {0,1,2,3,4}, --distribution {0,1,2,3,4}
                        The common distribution levels in MISP are as follows: 0: Your organization only - Default; 1: This community only; 2: Connected communities; 3: All communities; 4: Sharing
                        group.
```