---
layout: post
title: Test Page
date:   2015-06-04 13:50:39
categories: others
---


<div style="width:100%;height:0;padding-bottom:75%;position:relative;"><iframe src="https://giphy.com/embed/ClsZPj1jbbmcSTc942" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div><p><a href="https://giphy.com/gifs/ClsZPj1jbbmcSTc942">via GIPHY</a></p>
             

This is a test blog page where we can explore how to embedd images in the blog. 
![image](https://giphy.com/embed/ClsZPj1jbbmcSTc942)
             
<div style="width:100%;height:0;padding-bottom:75%;position:relative;"><iframe src="https://giphy.com/embed/ClsZPj1jbbmcSTc942" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div><p><a href="https://giphy.com/gifs/ClsZPj1jbbmcSTc942">via GIPHY</a></p>

<div style="width:100%;height:0;padding-bottom:75%;position:relative;"><iframe src="https://giphy.com/embed/ClsZPj1jbbmcSTc942" width="100%" height="100%" style="position:absolute" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div><p><a href="https://giphy.com/gifs/ClsZPj1jbbmcSTc942">via GIPHY</a></p>


![Browse_Georeference]([https://media.giphy.com/media/vFKqnCdLPNOKc/giphy.gif](https://giphy.com/embed/ClsZPj1jbbmcSTc942))

<iframe src="https://giphy.com/embed/ClsZPj1jbbmcSTc942" width="480" height="362" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/ClsZPj1jbbmcSTc942">via GIPHY</a></p>



![my alternate text]([http://lorempixel.com/400/200](https://pbs.twimg.com/profile_images/1455185376876826625/s1AjSxph_400x400.jpg));

## Image example 1

Here, I will embedd image from local assets which goes into `assets` directory in project's `root` directory. Choose a specific image, related to particular post. I chose to name the image `test-page-image-1.jpg`, which I will embedd as:

```markdown
![my alternate text](/assets/test-page-image-1.jpg);
``` 

![my alternate text](/assets/test-page-image-1.jpg);

Ofcourse, you can load images from web as well. Just point to image direct URL. For ex, here is one placeholder image:

```markdown
![my alternate text](http://lorempixel.com/400/200);
``` 

![my alternate text](http://lorempixel.com/400/200);

One cool thing about this is the fact that images adapt themselves to the screen size of device. Try to resize your browser window and check for yourself, Have fun.



---
layout: post
title: Example content for posts  
categories: others
---


<p><small>This demo page has been used from <a href="http://jasonm23.github.io/markdown-css-themes/" target="_blank">http://jasonm23.github.io/markdown-css-themes/</a>.</small></p>

<h1>A First Level Header</h1>

<h2>A Second Level Header</h2>

<h3>A Third Level Header</h3>

<h4>A Fourth Level Header</h4>

<h5>A Fifth Level Header</h5>

<h6>A Sixed Level Header</h6>

<p>Now is the time for all good men to come to
the aid of their country. This is just a
regular paragraph.</p>

<p>The quick brown fox jumped over the lazy
dog&rsquo;s back.</p>

<hr />

<h3>Header 3</h3>

<blockquote><p>This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.</p>

<p>Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.</p>

<h2>This is an H2 in a blockquote</h2>

<p>This is the first level of quoting.</p>

<blockquote><p>This is nested blockquote.</p></blockquote>

<p>Back to the first level.</p></blockquote>

<p>Some of these words <em>are emphasized</em>.
Some of these words <em>are emphasized also</em>.</p>

<p>Use two asterisks for <strong>strong emphasis</strong>.
Or, if you prefer, <strong>use two underscores instead</strong>.</p>

<ul>
<li>Candy.</li>
<li>Gum.</li>
<li>Booze.</li>
<li>Red</li>
<li>Green</li>
<li><p>Blue</p></li>
<li><p>A list item.</p></li>
</ul>


<p>With multiple paragraphs.</p>

<ul>
<li><p>Another item in the list.</p></li>
<li><p>This is a list item with two paragraphs. Lorem ipsum dolor
sit amet, consectetuer adipiscing elit. Aliquam hendrerit
mi posuere lectus.</p></li>
</ul>


<p>Vestibulum enim wisi, viverra nec, fringilla in, laoreet
vitae, risus. Donec sit amet nisl. Aliquam semper ipsum
sit amet velit.*   Suspendisse id sem consectetuer libero luctus adipiscing.</p>

<ul>
<li>This is a list item with two paragraphs.</li>
</ul>


<p>This is the second paragraph in the list item. You&rsquo;re
only required to indent the first line. Lorem ipsum dolor
sit amet, consectetuer adipiscing elit.</p>

<ul>
<li><p>Another item in the same list.</p></li>
<li><p>A list item with a bit of <code>code</code> inline.</p></li>
<li><p>A list item with a blockquote:</p>

<blockquote><p>This is a blockquote
inside a list item.</p></blockquote></li>
</ul>


<p>Here is an example of a pre code block</p>

<pre><code>tell application "Foo"
    beep
end tell
</code></pre>

<p>This is an <a href="#">example link</a>.</p>

<p>I start my morning with a cup of coffee and
<a href="http://www.nytimes.com/">The New York Times</a>.</p>

### Code snippet

{% highlight python %}
if __name__ =='__main__':
    img_thread = threading.Thread(target=downloadWallpaper)
    img_thread.start()
    st = '\rDownloading Image'
    current = 1
    while img_thread.is_alive():
        sys.stdout.write(st+'.'*((current)%5))
        current=current+1
        time.sleep(0.3)
    img_thread.join()
    print('\nImage of the day downloaded.')
{% endhighlight %}





<!DOCTYPE html>
<html>
  <head>
    {% include meta.html %}
      <link rel="alternate" type="application/rss+xml" title="RSS" href="/feed.xml">
      <script type="text/javascript">window.baseurl = '{{ site.url }}';</script>
      {% include css.html %}
  </head>

  <body class="home overflow-hidden">
    {% include header.html %}
    {% include main.html %}
    {% include js.html %}
    {% include analytics.html %}
  </body>
</html>


---
layout: default
---
<div class="well">
    {% if page.subtitle %}
    <h4 class="home-subtitle">{{ page.subtitle }}</h4>
    {% endif %}
    <div>
    	{{ content }}
    </div>
</div>


---
layout: default
---
<div class="post-content well">
<article class="content">
    <div class="post">{{ content }}</div>
    <hr />
    {% include share-page.html %}
</article>
<hr />
{% assign hasSimilar = '' %}
{% for post in site.posts  %}
    {% assign postHasSimilar = false %}
    {% for tag in post.categories %}
        {% for thisTag in page.categories %}
            {% if postHasSimilar == false and hasSimilar.size < 6 and post != page and tag == thisTag %}
                {% if hasSimilar.size == 0 %}
                <div class="panel-body">
                <h4>Related Posts</h4>
                <ul>
                {% endif %}
                <li class="relatedPost">
                    <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
                    {% if post.categories %}
                        <small>(Categories: {% for category in post.categories %}<a href="/category/{{ category }}">{{ category }}</a>{% if forloop.last == false %}, {% endif %}{% endfor %})</small>
                    {% endif %}
                </li>
                {% capture hasSimilar %}{{ hasSimilar }}*{% endcapture %}
                {% assign postHasSimilar = true %}
            {% endif %}
        {% endfor %}
    {% endfor %}
{% endfor %}
{% if hasSimilar.size > 0 %}
    </ul>
    </div>
{% endif %}

<div class="PageNavigation">
  {% if page.previous.url %}
    <a class="prev pull-left" href="{{ site.url }}{{ page.previous.url }}">&laquo; {{ page.previous.title }}</a>
  {% endif %}
  {% if page.next.url %}
    <a class="next pull-right" href="{{ site.url }}{{ page.next.url }}">{{ page.next.title }} &raquo;</a>
  {% endif %}
</div>


<div class="disqus-comments">
    <div id="disqus_thread"></div>
    <script type="text/javascript">
        /* <![CDATA[ */

        var disqus_shortname = "{{ site.disqus_shortname }}";
        var disqus_identifier = "{{ site.url }}_{{ page.title }}";
        var disqus_title = "{{ page.title }}";

        /* * * DON'T EDIT BELOW THIS LINE * * */
        (function() {
            var dsq = document.createElement('script'); dsq.type = 'text/javascript'; dsq.async = true;
            dsq.src = '//' + disqus_shortname + '.disqus.com/embed.js';
            (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(dsq);
        })();
    /* ]]> */
    </script>
</div>
</div>

---
layout: default
---
<div class="content well">
<header id="post-header">
    <h1 id="post-subtitle">Articles by category: <em class="text-muted">{{ page.categories }}</em></h1>
</header>

<div id="post-content">
    <hr />
    {% for category in site.categories %}
        {% capture category_slug %}{{ category | first }}{% endcapture %}
        {% for c_slug in category_slug %}
            {% if c_slug == page.categories %}
                <button class="btn btn-sm btn-primary btn-raised">{{ c_slug }}</button>
            {% else %}
                <a href="{{ site.baseurl }}/category/{{ c_slug }}" class="btn btn-sm btn-default btn-raised">{{ c_slug }}</a>
            {% endif %}
        {% endfor %}
    {% endfor %}
    <hr />

    {% if site.categories[page.categories] %}
    <div class="list-group">
        {% for post in site.categories[page.categories] %}
        <div class="list-group-item">
            <div class="row-action-primary">
              <i class="fa fa-sticky-note"></i>
            </div>
            <div class="row-content">
            {% capture post_year %}{{ post.date | date: '%Y' }}{% endcapture %}
            {% if forloop.first %}
                <div class="least-content">{{ post_year }}</div>
            {% endif %}
            
            {% if forloop.first == false %}
                {% assign previous_index = forloop.index0 | minus: 1 %}
                {% capture previous_post_year %}{{ site.categories[page.categories][previous_index].date | date: '%Y' }}{% endcapture %}
                {% if post_year != previous_post_year %}
                <div class="least-content">{{ post_year }}</div>
                {% endif %}
            {% endif %}
            <div class="least-content">{{ post.date | date_to_string }}</div>
            <h4 class="list-group-item-heading"><a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a></h4>
            <p class="list-group-item-text">{{ post.content | strip_html | truncatewords: 20 }}</p>
            
            </div>
        </div>
        <div class="list-group-separator"></div>
        {% endfor %}
    </div>
    {% else %}
        <p>There are no posts in this categories.</p>
    {% endif %}
</div>
</div>
Footer

---
layout: default
---
<article class="post">

  <div class="post-content">
    {{ content }}

    <div class="projects row">
    {% include project_tags.html %}
    {% for i in site.data.projects %}
    <div class="project-item col-md-4 col-sm-6 col-xs-12" data-tags='{{ i.tags | jsonify | downcase }}'>
    	<div class="well project-outer">
    		<div class="project-inner">
    			<a href="/static/projects/{{ i.image }}" class="thickbox">
    			<div class="project-img bordered" style="background-image: url('/static/projects/{{ i.image }}');"></div>
                </a>
                {% if i.url %} <a href="{{ i.url }}"> {% endif %}
    			<h3 class="project-headlines">{{ i.name }}</h3>
    			{% if i.url %} </a> {% endif %}
    			<div class="project-content">
    				<div class="tag-holder">
    				{% if i.tags %} 
    					{% for j in i.tags %}
    					<span class="label tags tag-filter" data-tag="{{ j | downcase }}">{{ j }}</span>
    					{% endfor %}
    				{% endif %}
    				</div>
    				
    			</div>
    			<div class="project-footer"> 
    				{% if i.url %} 
    				<a href="{{ i.url }}" class="btn btn-info btn-raised btn-sm project-link">View</a>
    				{% endif %}
    				<span class="project-timeline">{{ i.date }}</span>
    			</div>
    		</div>
    	</div>
        </div>
    {% endfor %}
    </div>
  </div>

</article>
