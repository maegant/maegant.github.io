---
title: "Website Design"
layout: page
category: fun
img: images/portfolio/website/mm-layout-splash.png
description: "Tutorial on creating a website using Jekyll+Github Pages "
usemathjax: true
---

I built this website (code available on my [github](https://github.com/maegant/website)) using Jekyll. Since I know it can seem daunting to get into building custom websites, I'll outline the steps I took.

## Step 1: Create a 'Github Pages' repository to host your website:
I choose to host my website using github pages. To set this up, I followed the instructions [here](https://pages.github.com/), specifically for the 'User or organization site'.                                       

## Step 2: Populate repository with Jekyll site:
There are many ways to create your website, all of which can be hosted by Github Pages. In the past, I directly coded HTML code to create my website. However, I eventually found this hard to edit and update as my website content evolved. Thus, to more easily update my website, I switched to using [Jekyll](https://jekyllrb.com/). The main benefit of Jekyll is that it hides most of the HTML code in the backend, allowing you to focus on the actual content of your website. It is also easily customized and has many already developed layouts.

To get started with Jekyll, follow the quickstart guide [here](https://jekyllrb.com/docs/).

### What I actually did (on Ubuntu 18.04 and using ['Minimal-Mistakes'](https://mmistakes.github.io/minimal-mistakes/) Jekyll theme):

Inside of my Github repository, I did the following to setup my website:

1. Install Ruby:
  ```
  sudo apt-get install ruby-full build-essential
  ```

2. Install RubyGems
  ```
  sudo gem update --system
  ```

3. Install GCC and Make
  ```
  sudo apt update
  sudo apt install build-essential
  gcc --version
  make -version
  ```

4. Install Jekyll
  ```
  sudo apt-get install ruby-full build-essential zlib1g-dev
  echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
  echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
  echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
  source ~/.bashrc
  gem install jekyll bundler
  ```

5. Download [minimal mistakes](https://github.com/mmistakes/minimal-mistakes) and place the contents of the website into your Github repository. Other Jekyll themes are available [here](https://jekyllrb.com/resources/).

6. Remove the unnecessary components of the Minimal Mistakes contents by removing the following folders and files:
- .editorconfig
- .gitattributes
- .github
- /docs
- /test
- CHANGELOG.md
- minimal-mistakes-jekyll.gemspec
- README.md
- screenshot-layouts.png
- screenshot.png

7. Install Jekyll paginate for minimal mistakes:
  ```
  gem install jekyll-paginate
  ```

8. Replace the contents of the Gemfile with:
  ```
  source "https://rubygems.org"
  gem "jekyll"
  gem "minimal-mistakes-jekyll"
  ```

9. Fetch and update bundled gems
  ```
  bundle
  ```

10. Build the website:
```
jekyll build
```

## Step 3: Preview website:
You can preview by the website by running:
```
jekyll serve
```
and then visiting http://127.0.0.1:4000

As you edit the contents of the website, you will be able to view the live changes by simply refreshing http://127.0.0.1:4000

