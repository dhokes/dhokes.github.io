---
layout: post
title: Using Tags in Jekyll
tags:
- jekyll
---

After considering various options, I decided to host this blog using [GitHub Pages](https://pages.github.com/).  I found a theme called [Hyde](http://hyde.getpoole.com/) that I liked so I thought I'd use that rather than spending time designing something from scratch. At a later date, I might create my own.

However, GitHub Pages only supports several Jekyll plugins and as a result, I've had to create a solution to enable to me to add tags to posts.

I can add tags to each post's YAML frontmatter:
<pre>
<code>
layout: post
title: Using Tags in Jekyll
tags:
- jekyll
</code>
</pre>

For each new tag I want to use, I create a simple html file like the following for file for the 'jekyll' tag:


<code>/tags/jekyll/index.html</code>

This html file contains the following content:

<pre>
<code>
---
layout: tagpage
tag: jekyll
---
</code>
</pre>
