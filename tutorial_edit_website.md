
# Struc_Eng_Library_Website

This website is built with [mkdocs](https://www.mkdocs.org/). A [Github Runner](https://github.com/kfmResearch-NumericsTeam/Struc_Eng_Library_Website/actions/workflows/deploy.yml) will redeploy the website on a new commit.

## Edit website 
Navigation hierarchy is changed in mkdocs.yml file. It resembles the file structure in the ./docs folder.  

<p align="left">
<img src="https://user-images.githubusercontent.com/2311941/196964646-1871193b-8af9-4129-94d0-f02bd015379e.png" alt="strucenglib" width="400"/>
</p>

## Edit a Page
The content pages are written in markdown and are available in the ./docs folder.
Edit a markdown file in the Github file editor. Changes are redeployed upon a new commit.

<p align="left">
<img src="https://user-images.githubusercontent.com/2311941/196965370-33f40404-eb83-4015-a1c6-c1cc770aa6ff.png" alt="strucenglib" width="400"/>
</p>


## Markdown Documentation
https://squidfunk.github.io/mkdocs-material/reference/images/


## Developer Notes
### Local Build
If you prefer to edit the website locally without Github's UI, execute the following commands.

Install python 3 and pip.

```sh
# 1. create new virtual environment (optional)

# 2. install dependencies
pip install -r ./github/requirements.txt

# 3. serve content
mkdocs serve

```

### Installed Runners
- [![Build Website](https://github.com/kfmResearch-NumericsTeam/Struc_Eng_Library_Website/actions/workflows/deploy.yml/badge.svg)](https://github.com/kfmResearch-NumericsTeam/Struc_Eng_Library_Website/actions/workflows/deploy.yml): Builds website with mkdocs  
- [![pages-build-deployment](https://github.com/kfmResearch-NumericsTeam/Struc_Eng_Library_Website/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/kfmResearch-NumericsTeam/Struc_Eng_Library_Website/actions/workflows/pages/pages-build-deployment): Deploys website with Github Pages  


