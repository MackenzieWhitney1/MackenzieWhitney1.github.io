---
title: "Getting started with Jekyll"
categories:
  - Blog
tags:
  - helloworld
  - beginner
  - jekyll
---
> "All things are difficult before they are easy." <cite><a href="https://www.brainyquote.com/quotes/thomas_fuller_125402">Thomas Fuller</a></cite>

The good news is that it's a lot like other templating languages like Pug.
{: .notice--success}
I will not talk about the downsides.
{: .notice--danger}

Steps to Configure GitHub Pages
- There is a tutorial on GitHub to create one from scratch, but it can be daunting. A template provides structure and features like tags and search.
- Fork https://github.com/mmistakes/mm-github-pages-starter as #UserName.github.io
- To setup IntelliJ, you need to:
1. Install Ruby
2. In a command prompt, install Jekyll and Bundler: gem install jekyll bundler
3. Navigate to the directory path where you've forked your repo
4. Execute the command bundle install. It will not work if the directory doesn't have a Gemfile. (A Gemfile describes dependencies in Ruby.)

Note: You might have to comment out this line from the Gemfile like so: # gem "wdm", "~> 0.1.0" if Gem.win_platform?
{: .notice--warning}

5. Open VSCode.
6. In the Developer Command Prompt (Power Shell), run "bundle exec jekyll serve".

Note: Page refreshes don't catch all changes made so you might have to CTRL+C to terminate and redeploy sometimes. (config.yaml especially)
{: .notice--warning}

7. You can then access the site http://localhost:4000

If you do have a repo called #UserName.github.io, you should be able to access it as a link
ex. https://UserName.github.io

8. Also be sure to add a .gitignore file if you have a .vs folder since git doesn't like this.