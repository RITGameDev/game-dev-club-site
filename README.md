# Game Dev Club Site

## Getting Started

The site is built with [Jekyll](https://jekyllrb.com/docs/), a static website generator running off of Ruby. 

To get started with running Jekyll, just follow the instructions on their website [here](https://jekyllrb.com/docs/installation/)

## Contribution Guide

If you want to make changes to the site there are a couple of things to consider: 

Do your work on a seperate branch with a meaningful name, i.e. `update-location` or `change-logo`. 

When you are done with your changes, then simply make a pull request to `master`
and the PR will undergo a review, and then be merged in if successful. 

Do you want to add a game to our showcase? Just make a PR with your post file in the `_posts` folder. 
If you are having trouble with this or have questions then you can use the 
[AurumKings](https://github.com/RITGameDev/game-dev-club-site/blob/master/_posts/2019-03-07-aurum-kings.markdown) post as an example. 
If you need further help then feel free to reach out on our [Discord](https://discord.gg/BwU7QBA)! 

If you have a change to the core site (i.e. CSS stylings that effect more than just your post, layout options, etc) then feel free to make an issue with what you think should change! 


### Jekyll Quick Start

I always forget the commands for installing Jekyll and getting the enviornment setup. 
Here they are!  

#### Ubuntu

For Ubuntu, use the following commands to install jekyll and ruby and get 
the site up and running locally! 

```
sudo apt-get install ruby ruby-dev build-essential

echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME=$HOME/gems' >> ~/.bashrc
echo 'export PATH=$HOME/gems/bin:$PATH' >> ~/.bashrc
source ~/.bashrc
```

```
gem install jekyll bundler
```

```
gem sources --add https://rubygems.org/
```

Confirm your ruby install

```
ruby -v
```

If you run into issues try this command:

```
bundle update jekyll
gem update jekyll
```

To run Jekyll:
```
jekyll serve --watch
```