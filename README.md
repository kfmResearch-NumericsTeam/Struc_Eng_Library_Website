[![Publish docs via GitHub Pages](https://github.com/kfmResearch-NumericsTeam/Struc_Eng_Library_Website/actions/workflows/deploy.yml/badge.svg)](https://github.com/kfmResearch-NumericsTeam/Struc_Eng_Library_Website/actions/workflows/deploy.yml)

# StrucEng Library Project

Welcome to the StrucEng Library. If you landed here from our website https://strucenglib.ethz.ch/, here is an overview of the most important repositories:
- Website (this site): [Struc_Eng_Library_Website](https://github.com/kfmResearch-NumericsTeam/Struc_Eng_Library_Website)
- Rhino 3d plugin: [StrucEng_Library_Plug_in](https://github.com/kfmResearch-NumericsTeam/StrucEng_Library_Plug_in)
- Connection layer for remote setup: [Struc_Eng_Library_Server](https://github.com/kfmResearch-NumericsTeam/Struc_Eng_Library_Server)
- Snippet collection: [StrucEng_Library](https://github.com/kfmResearch-NumericsTeam/StrucEng_Library)

---- 

## How to Edit a Page
This website is built with [mkdocs](https://www.mkdocs.org/). A [Github Runner](https://github.com/kfmResearch-NumericsTeam/Struc_Eng_Library_Website/actions/workflows/deploy.yml) will redeploy the website on a new commit.

### Edit Navigation
Navigation hierarchy is changed in mkdocs.yml file. It resembles the file structure in the ./docs folder.  

<p align="left">
<img src="https://user-images.githubusercontent.com/2311941/196964646-1871193b-8af9-4129-94d0-f02bd015379e.png" alt="strucenglib" width="400"/>
</p>

### Edit a Page
The content pages are written in markdown and are available in the ./docs folder.
Edit a markdown file in the Github file editor. Changes are redeployed upon a new commit.

<p align="left">
<img src="https://user-images.githubusercontent.com/2311941/196965370-33f40404-eb83-4015-a1c6-c1cc770aa6ff.png" alt="strucenglib" width="400"/>
</p>


## Mkdocs Markdown Documentation
https://squidfunk.github.io/mkdocs-material/reference/images/


## Local Build

Install python 3 and pip.

```sh
# 1. create new virtual environment (optional)

# 2. install dependencies
pip install -r ./github/requirements.txt

# 3. serve content
mkdocs serve

```


## Files and Directories
```
./docs..........: Markdown files
./docs/assets...: Static assets
./overrides.....: html files to overwrite default template
./mkdocs.yml....: config file
```

