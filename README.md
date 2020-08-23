# Personal Website

Source content used to generate my personal site - https://alexpnt.github.io/

### Installation

#### Install node and npm using nvm

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash

# in a new shell, install the latest version of node
nvm install node 
```

#### Install pandoc

```
# example for ubuntu-based distributions
wget https://github.com/jgm/pandoc/releases/download/2.10.1/pandoc-2.10.1-1-amd64.deb
sudo dpkg -i pandoc-2.10.1-1-amd64.deb
```

#### Install hexo site project

```
cd site
npm install
```

#### Serving
```
hexo server
```
### Tools:

* [hexo](https://hexo.io/) - A fast, simple & powerful blog framework.
* [cactus-dark](https://github.com/probberechts/cactus-dark) - A responsive, dark and simple theme for Hexo. 
* [pandoc](https://github.com/jgm/pandoc) - Universal markup converter. 