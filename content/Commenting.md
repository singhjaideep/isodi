Title: Big deal with Commenting
Date: 2017-01-21 21:51
Category: Blog

I would love to add comments to this blog. But there are a few hiccups. This is a static blog, hosted on github pages, so its not simple as it seems. I explored various avenues to add commenting, taking into account different factors. Here are what my options boil down to:

1. Third party services like Disqus,facebook etc.
    * Pros: Easiest to integrate, lot of "social" tools.
    * Cons: Javascript, external scripts, users need to create account
2. [Isso](https://posativ.org/isso/) : Simple commenting system backed by SQLite
    * Pros: No external js needed.
    * Cons: Github doesn't allow sql of anytime on github pages.. so nope
3. [Super duper hack using github API, issues and posthooks](http://ivanzuzak.info/2011/02/18/github-hosted-comments-for-github-hosted-blogs.html)
    * Pros: Hard to implement, but good learing exprience
    * Cons: Hard to implement, users require github cred
4. [Roll my own commenting system using Firebase](https://codepen.io/joshbivens/pen/jbNJJR)
    * Pros: Firebase handles all sql stuff
    * Cons: Need to maintain spam rules and other stuff
5. [Static comments hack via email](https://bernhard.scheirle.de/posts/2014/March/29/static-comments-via-email/)
    * Pros: Users just need an email, no account needs to be created
    * Cons: Pretty barbaric don't you think?

Out of all these I liked 4 and 5. I like 4 more because its more user friendly, and I can think off all the spam detection stuff later. If its too hard to setup I'll go with 5.