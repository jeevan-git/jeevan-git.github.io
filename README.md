# Run this project 🏃

## For local run

### Install dependencies
```shell
sudo apt-get install ruby ruby-dev make build-essential
sudo gem install -V bundler
bundle
```

### Run jekyll locally
```shell
make
```
-------------------------------------------------------------------

# About ```_config.yml``` file

*  All setup are done in ```_config.yml``` file

**Important note : main file is ```_config.yml``` file ho so tyo file ma kai update garyasi mathi github ko line ma herhani pass vaya ki vavyana  vanyara**

-----------------------------------------------------------------


After config ```config.yml``` file we will move in creating pages, posts, and collections.
# Creating a pages

##  Goto _data and add title and url
```
main:
  - title: "Posts"
    url: /posts/
  - title: "Post collections"
    url: /postcollections/
  - title: "About"
    url: /about/
    
```
##  Goto _pages folder and create pages.
```
permalink: /about/
title: "About"
classes: wide
excerpt: Learn about me, who iam and what I do.

```

**Be sure the permalink = url  in navigation.yml file.**

Note: page ma click garni bitikai auni banaunai kura haru yahi lekhni .
Yadi post haru lekhnu x vanya post ma lekhni.

-----------------------------------------------------------------

#  Creating posts

##  Goto _posts folder and create posts.
* Note while creating posts we  need to focus on first setion.

## Note while writing post

## Directly write in markdown

* Write simple text directly.
* --- is for horizontal line
```python
 print("hello")
```
##  Things need while writing posts

* For image you can use : [draw.io](https://app.diagrams.net/)
* For emoji : [emojipedia](https://emojipedia.org/)
* For githubcard  : [githubcard](https://ghlinkcard.com/)
* For weights : [shild](https://shields.io/)

-----------------------------------------------
# Page and post
* Note :  if page, post,.yml, or j ni git ma properly configuration vayo vanya thyakka mathi bar ma yellow point dekhinxa github action pass vanyara.
* ![image](https://github.com/MadanBaduwal/MadanBaduwal.github.io/blob/main/images/info.png)
* page ma classes: wide vanyara hunxa 
* post ma layout : categories,posts  vanyara hunxa.


----------------------------------------------------------

# Creating a collections 
**Note: projects / talks / session ... haruko collection banauna ko lagi**

* Goto the ```_data``` > navigation.yml file and create new pages with new title and  url.
* Goto the ```_pages`` folder and create new .html file (eg: portfolio-archive.html) note page url = permalink of this .html file
* Write collection in ``_post`` folder




----------------------------------------------------------------
Note : website lai akchoti search engine ma verify garayo vanya pugxa.

