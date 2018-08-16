---
ID: 226
post_title: 'Deployment and SSH keys in Bitbucket'
post_name: deployment-and-SSH-keys-in-Bitbucket
author: Karen Geerts
post_date: 2018-08-16 21:30:00
layout: posts
published: true
tags: [ ]
categories:
  - Uncategorized
---
The other day, I decided to continue working my way through the Michael Hartl's <a href="https://www.railstutorial.org/book/frontmatter">Rails tutorial</a>
I started a few months ago but then life got in the way I guess, and I got distracted trying to get my head around Python and SQL.

This tutorial recommends using AWS Cloud9 IDE instead of running everything locally. Since I'm using more than 1 laptop, I thought it made sense to follow this recommendation so I could easily continue working without having to worry about differences in versions etc. Unfortunately, trying to get it all to work took a lot longer than it should have.
Setting up a Cloud9 IDE environment was easy enough, the pain (for me) was connecting to a Bitbucket repository.

The tutorial refers to this website that explains how everything is done: <a href="https://confluence.atlassian.com/bitbucket/set-up-an-ssh-key-728138079.html" target="_blank">Atlassian Bitbucket official doco</a>

Everything on this website is 100% correct, but it was made insufficiently clear that the SSH key had to be added to your own user account instead of the repository setting. So: if you have just create a repo and still have that window open, ignore the word "settings" that is shining at you. Locate your user avatar (left hand side of the screen, all the way at the bottom for maximum chances of not seeing it at all). Click on your avatar and then select 'Bitbucket-settings' - it's there where you then add the SSH key.

The description  <a href="https://confluence.atlassian.com/bitbucketserver0510/ssh-user-keys-for-personal-use-951390557.html" target="_blank">here</a> makes a lot more sense - but I only found it after extensive Googling the error message I received about a deployment key.

And while on the subject, a <a href="https://medium.com/@obrientimothya/developing-ruby-on-rails-5-1-apps-with-the-aws-cloud9-ide-18826ae1426b" target="_blank">Medium blog post</a> I wished I had found earlier about Cloud9 and running Rails apps : 