---
title: 'Hello,World!'
date: 2017-04-03 12:23:14
tags: Hexo Git VPS
---
Hello,World!

This is my first Hexo blog,which is hosted on my vps,driven by the hexo blog frame and auto updated with git-hooks.

Here i put down the basical steps to achieve that:

A, Get the VPS running with nginx and git installed,to be configured later;

B, Prepare a dedicated account such as hexo to manage the hexo blog for convience;

C, Initiate a git repository to be synchronized from the local hexo folder to;

D, Locally install the nvm for the npm installation,and then the npm,which is the node.js manager,and then install hexo-cli with the npm;

E, Locally initiate the working folder,whatever the name is,followed by "hexo init <folder> && cd <folder> && npm install && npm install hexo-deployer-git --save".

F, On the VPS,in the Git repo,config the post-receive git-hooks for to synchronize the VPS git repo from the nginx <WWW> working folder;

G, On the VPS,configure the nginx running scripts,details vary much;

H, Locally generate the ssh key and upload the pub key to the VPS for hexo-deployer-git to auto login without passphrase input,On the VPS ssh authorized_keys should be configured,details to be checked and more related to the ssh subject so neglected;

I, The finishing touch,config the _config.yml the deploy part at the end of the file,make it connected to the VPS git repository;

J, Locally in the hexo initiated <folder>,type"hexo new post "My firest article."" and "vim ./source/_posts/My-first-article.md" to put down your blog...

   

