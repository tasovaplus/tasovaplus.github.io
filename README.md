# TASOVA Plus website

> The website for the TASOVA Plus network.

---

## What is this?

This is a Jekyll-based website for the TASOVA Plus network. This repository comprises templates and files with the content. The real website is generated from these files using the [Jekyll static-website generator](https://jekyllrb.com) and the [minimal mistakes template](https://mmistakes.github.io/minimal-mistakes).

The TASOVA Plus website is deployed in [Github Pages](https://pages.github.com/). This site is inspired in [AcademicPages/events](https://github.com/academicpages/events), a fork from the [minimal mistakes template](https://mmistakes.github.io/minimal-mistakes). 

## Local installation for development

You can install Jekyll on your computer to preview the changes before pushing them to the Github repository. 

The following are instructions for Ubuntu Linux (or Ubuntu/WSL on Windows 10)

1. Install Jekyll pre-requisites, including the Ruby language

   ```
   sudo apt-get install ruby-full build-essential zlib1g-dev
   ``` 

2. Configure the Ruby language to install software in the `$HOME` directory 

   ```
   echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
   echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
   echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
   source ~/.bashrc
   ``` 

3. Install Jekyll

   ```
   gem install jekyll bundler
   ``` 

3. Download the website

   ```
   git clone https://github.com/tasovaplus/tasovaplus.github.io.git
   ``` 

4. Install additional libraries required by Jekyll

   ```
   cd tasovaplus.github.io
   bundle install
   ``` 

5. Run the Jekyll preview to preview and regenerate the website when the files are changed

   ```
   bundle exec jekyll serve
   ``` 

5. Preview the site using a web browser

   ```
   http://localhost:4000
   ``` 
   
---

### Licenses

This website uses the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes) that is licensed using [The MIT License (MIT)](https://opensource.org/licenses/MIT).