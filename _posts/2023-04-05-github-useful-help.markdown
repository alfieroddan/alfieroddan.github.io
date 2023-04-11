---
layout: post
title: Useful Notes for Github Pages
author: Alfie Roddan
---

# Start your own Jekyll / Github blog
## Startup using:
- [This startup jekyll](https://www.aleksandrhovhannisyan.com/blog/getting-started-with-jekyll-and-github-pages/#how-to-set-up-github-pages)
- [This example gitpage](https://github.com/ian-whitestone/ian-whitestone.github.io)

Note I don't use the minima theme as I want to use MathJax. I simply copied the minima theme files from `bundle info --path minima`. Make sure to add the [SEO Plugin](seo-plug)!

[seo-plugin]: https://github.com/jekyll/jekyll-seo-tag/blob/master/docs/installation.md


# MathJax
To use mathjax add to the `_layouts/post.html`:

```html
<script>
  MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']]
    }
  };
  </script>
  <script id="MathJax-script" async
    src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js">
  </script>
```

This will render all math like you would in latex or markdown (escape using `$`).

Now  \\$x_{2}\\$ becomes $x_{2}$ with no extra effort!


# From Jekyll
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

Jekyll requires blog post files to be named according to the following format:

`YEAR-MONTH-DAY-title.MARKUP`

Where `YEAR` is a four-digit number, `MONTH` and `DAY` are both two-digit numbers, and `MARKUP` is the file extension representing the format used in the file. After that, include the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/