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

# Google Custom Search Engine 
*  follow [minimal mistake](https://mmistakes.github.io/minimal-mistakes/docs/configuration/)
 *  Create a New search engine in [Google Custom Search Engine](https://cse.google.com/cse/all) tya bata ako cx="YOUR_SEARCH_ENGINE_ID" lai ```__config.yml ``` ko google: search_engine_id: YOUR_SEARCH_ENGINE_ID  ma past gardeni.
 ---------------------------------------------------------------
 
# SEO, and analytics settings 

**Note : different search engine ma afno site verify garnuparni ani tyo search tool le afai khojxa , there are lots of search engine tool**

## SEO( talko searching tool use garni)

### [Google Search Console](https://search.google.com/)
* 1-day, 2-day jati time lagxa verify huna
* google search engine ma visiable  banauna , google search console ma verify garaunu parxa/ yadi google analytics ma verify garisakeko x vanya yasma garnu pardaina
* Formerly known as Google Webmaster Tools, add your verification code in ```___config.yml``` like so: google_site_verification: "yourVerificationCode"

### [Bing Webmaster Tools](https://www.bing.com/webmasters/help/add-and-verify-site-12184f8b?tid=ef68211b-35d5-438b-985b-27519fb3ce32#) 
* Bing ma website visiable banauna yo chai(google search console jastai arko tool ho yo)
* Bing webmaster tools ma site add garni [2 tarika xan](https://www.bing.com/webmasters/home) , akchoti google console ma add garisakyasi tya verify vaisakeko x vanya bing ma google search console ko help le site lai bing webmaster tools ma add garna sakinxa 
* or manully ni add garna sakixa

Note : There  are lots of search engine tool ok.

## analytics settings (website ma kati traffic ayo sabai herna milxa ..)

* [	Google Standard Analytics](https://marketingplatform.google.com/about/analytics/)


---------------------------------------------------------------
# For custome domain 
If you have a custome domain(eg: madan.com) you can config your DNA to github as shown below.
We are going to config .np domain here in cloudflare, similiarly you can config in any DNS server.

Note 📝 : .np domain have no option CNAME so we use cloudflare
