---
layout: post
title: How to Start Using This Blog 
author: Kaushal
---

This Blog Post Would help you understand the flow of Construction of this blog and let you teach you things need to write your first blog in "gang-press"

#### How did we do it !

The whole blog was constructed with a two open source components:

* [Jekyll](http://jekyllrb.com/) - This is a static site generator. Which we have used to construct our blog.

* [Type Theme](https://rohanchandra.github.io/project/type/) - This is a jekyll  Template which we have used as a base to construct our blog  

#### Directory Structure of the blog

The most important thing to understand in publishing a post in Jekyll based blog is understanding the directory structure of the code. Here is the directory structure for Jekyll 

![Jekyll_directory_structure](/gang-press/img/posts/2015-02-15/jekyll_directory_structure.png)

* [_includes](http://github.com/wethegang/gang-press/tree/gh-pages/_includes) - This folder holds the components which would be reused again and again in posts page and also index page. Eg. header.html, footer.html.

* [_layouts](https://github.com/wethegang/gang-press/tree/gh-pages/_layouts) - This folder has all the HTML elements which control the layouts of the blog. This folder would have files like default.html, page.html and post.html.

* [_posts](https://github.com/wethegang/gang-press/tree/gh-pages/_posts) - This is the main folder which would have all of the posts in markdown with a specific naming convention. All posts should be named as " YYYY-MM-DD-title-of-the-blog.md ".

* [_sass](https://github.com/wethegang/gang-press/tree/gh-pages/_sass) - This has all the style components all grouped under _includes, _layouts and _posts.

* [css](https://github.com/wethegang/gang-press/tree/gh-pages/css) - This has a main style file which imports all the style components from _sass.

#### How to publish a blog post

Its very easy to create a blog post, Just create a markdown file and place it in "_posts" with a specific name. jekyll will take care of the rest.
Here are the  step by step instructions of doing the above with suitable references.

1. Create the blog post in [MarkDown](http://daringfireball.net/projects/markdown/)

2. name the blog posts in this format " YYYY-MM-DD-title-of-the-blog.md ".

3. Place the blog post in _posts directory of the repository and before placing, follow these steps

* Clone the repository 
{% highlight bash %}
git clone https://github.com/wethegang/gang-press.git 
{% endhighlight %}
*  Now move the markdown file to _posts directory of the repo
{% highlight bash %}
mv YYYY-MM-DD-title-of-the-blog.md gang-press/_posts/
{% endhighlight %}
*  Add the repository to the code
{% highlight bash %}
git add YYYY-MM-DD-title-of-the-blog.md 
{% endhighlight %}
*  commit the repositary, pull and push the repository
{% highlight bash %}
git commit -m "<message>"
git pull
git push
{% endhighlight %}

#### Preview your blog

Previewing is a bit difficult, because you need to have jekyll installed locally. Here are the instructions to set your environment as soon as  possible and start blogging.

* follow these instructions for installation of jekyll ([Instructions](http://jekyllrb.com/docs/installation/))

* Clone the repository 
{% highlight bash %}
git clone https://github.com/wethegang/gang-press.git 
{% endhighlight %}

* Go to the root of the repository and use jekyll to construct a local copy of the blog and host it in the local server
{% highlight bash %}
cd gang-press
jekyll serve
{% endhighlight %}

* Open the browser and connect to local host
{% highlight bash %}
google-chrome
http://localhost:4000/gang-press/
{% endhighlight %}

This should allow to see the preview. Keep writing new blogs and Happy blogging.
