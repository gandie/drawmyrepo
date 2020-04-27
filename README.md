# drawmyrepo - draw fancy diagrams from your git repo

Didn't find a tool to draw a diagram showing commits per month. So i wrote one.

Hope its useful.

# Installation

Debian Package requirements:

```bash
sudo apt-get install python3-matplotlib python3-tk
```

**Python3 is required!**

Python Package:

```bash
pip install -r requirements.txt
python setup.py install
```

Debian Package:

```bash
dpkg-buildpackage -us -uc
sudo dpkg -i ../python3-drawmyrepo_<your_version>.deb
```

# Usage

```plaintext
usage: drawmyrepo [-h] [-p PATH] [--from-year FROM_YEAR] [--to-year TO_YEAR]

optional arguments:
  -h, --help            show this help message and exit
  -p PATH, --path PATH  Path to git repo. Default is current workdirectory.
  --from-year FROM_YEAR
                        Year to start counting from. Default is 2014.
  --to-year TO_YEAR     Year to stop counting. Default is now.
```
