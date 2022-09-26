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
[
	{
		"name": "Cool project 1",
		"image": "placeholder.jpg",
		"url": "#",
		"date": "Jan 2014",
		"tags": ["Angular JS","API"]
	},
	{
		"name": "Cool project 2",
		"image": "placeholder.jpg",
		"url": "#",
		"date": "May 2014",
		"tags": ["Android","PHP"]
	},
	{
		"name": "Cool project 3",
		"image": "placeholder.jpg",
		"url": "#",
		"date": "June 2014",
		"tags": ["HTML","JQuery","PHP"]
	},
	{
		"name": "Cool project 4",
		"image": "placeholder.jpg",
		"date": "Oct 2016",
		"tags": ["Android","nodejs"]
	}

]
[
  {
    "text": "Home",
    "url": "/",
    "icon": "fa-home",
    "layout": "post"
  },
  {
    "text": "About",
    "url": "/about/",
    "icon": "fa-comments"
  },
  {
    "text": "Projects",
    "url": "/projects",
    "icon": "fa-desktop"
  },
  {
    "text": "Resume",
    "url": "/#",
    "icon": "fa-graduation-cap",
  },
  {
    "text": "Github",
    "url": "/#",
    "icon": "fa-github"
  },
  {
    "text": "XML Feed",
    "url": "/feed.xml",
    "icon": "fa-feed",
    "target": _blank
  }
]
