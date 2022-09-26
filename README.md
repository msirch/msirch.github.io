

theme                  : "minimal-mistakes-jekyll"
remote_theme           : "mmistakes/minimal-mistakes"
minimal_mistakes_skin    : "default" # "air", "aqua", "contrast", "dark", "dirt", "neon", "mint", "plum", "sunrise"

# Site Settings
locale                   : "en-US"
title                    : "Site Title"
title_separator          : "-"
subtitle                 : # site tagline that appears below site title in masthead
name                     : "Your Name"
description              : "An amazing website."
url                      : # the base hostname & protocol for your site e.g. "https://mmistakes.github.io"
baseurl                  : # the subpath of your site, e.g. "/blog"
repository               : # GitHub username/repo-name e.g. "mmistakes/minimal-mistakes"
teaser                   : # path of fallback teaser image, e.g. "/assets/images/500x300.png"
logo                     : # path of logo image to display in the masthead, e.g. "/assets/images/88x88.png"
masthead_title           : # overrides the website title displayed in the masthead, use " " for no title
# breadcrumbs            : false # true, false (default)
words_per_minute         : 200
comments:
  provider               : # false (default), "disqus", "discourse", "facebook", "staticman", "staticman_v2", "utterances", "giscus", "custom"
  disqus:
    shortname            : # https://help.disqus.com/customer/portal/articles/466208-what-s-a-shortname-
  discourse:
    server               : # https://meta.discourse.org/t/embedding-discourse-comments-via-javascript/31963 , e.g.: meta.discourse.org
  facebook:
    # https://developers.facebook.com/docs/plugins/comments
    appid                :
    num_posts            : # 5 (default)
    colorscheme          : # "light" (default), "dark"
  utterances:
    theme                : # "github-light" (default), "github-dark"
    issue_term           : # "pathname" (default)
  giscus:
    repo_id              : # Shown during giscus setup at https://giscus.app
    category_name        : # Full text name of the category
    category_id          : # Shown during giscus setup at https://giscus.app
    discussion_term      : # "pathname" (default), "url", "title", "og:title"
    reactions_enabled    : # '1' for enabled (default), '0' for disabled
    theme                : # "light" (default), "dark", "dark_dimmed", "transparent_dark", "preferred_color_scheme"
  staticman:
    branch               : # "master"
    endpoint             : # "https://{your Staticman v3 API}/v3/entry/github/"
reCaptcha:
  siteKey                :
  secret                 :
atom_feed:
  path                   : # blank (default) uses feed.xml
  hide                   : # true, false (default)
search                   : # true, false (default)
search_full_content      : # true, false (default)
search_provider          : # lunr (default), algolia, google
lunr:
  search_within_pages    : # true, false (default)
algolia:
  application_id         : # YOUR_APPLICATION_ID
  index_name             : # YOUR_INDEX_NAME
  search_only_api_key    : # YOUR_SEARCH_ONLY_API_KEY
  powered_by             : # true (default), false
google:
  search_engine_id       : # YOUR_SEARCH_ENGINE_ID
  instant_search         : # false (default), true
# SEO Related
google_site_verification :
bing_site_verification   :
naver_site_verification  :
yandex_site_verification :
baidu_site_verification  :

# Social Sharing
twitter:
  username               :
facebook:
  username               :
  app_id                 :
  publisher              :
og_image                 : # Open Graph/Twitter default site image
# For specifying social profiles
# - https://developers.google.com/structured-data/customize/social-profiles
social:
  type                   : # Person or Organization (defaults to Person)
  name                   : # If the user or organization name differs from the site's name
  links: # An array of links to social media profiles

# Analytics
analytics:
  provider               : false # false (default), "google", "google-universal", "google-gtag", "custom"
  google:
    tracking_id          :
    anonymize_ip         : # true, false (default)


# Site Author
author:
  name             : "Your Name"
  avatar           : # path of avatar image, e.g. "/assets/images/bio-photo.jpg"
  bio              : "I am an **amazing** person."
  location         : "Somewhere"
  email            :
  links:
    - label: "Email"
      icon: "fas fa-fw fa-envelope-square"
      # url: "mailto:your.name@email.com"
    - label: "Website"
      icon: "fas fa-fw fa-link"
      # url: "https://your-website.com"
    - label: "Twitter"
      icon: "fab fa-fw fa-twitter-square"
      # url: "https://twitter.com/"
    - label: "Facebook"
      icon: "fab fa-fw fa-facebook-square"
      # url: "https://facebook.com/"
    - label: "GitHub"
      icon: "fab fa-fw fa-github"
      # url: "https://github.com/"
    - label: "Instagram"
      icon: "fab fa-fw fa-instagram"
      # url: "https://instagram.com/"

# Site Footer
footer:
  links:
    - label: "Twitter"
      icon: "fab fa-fw fa-twitter-square"
      # url:
    - label: "Facebook"
      icon: "fab fa-fw fa-facebook-square"
      # url:
    - label: "GitHub"
      icon: "fab fa-fw fa-github"
      # url:
    - label: "GitLab"
      icon: "fab fa-fw fa-gitlab"
      # url:
    - label: "Bitbucket"
      icon: "fab fa-fw fa-bitbucket"
      # url:
    - label: "Instagram"
      icon: "fab fa-fw fa-instagram"
      # url:


# Reading Files
include:
  - .htaccess
  - _pages
exclude:
  - "*.sublime-project"
  - "*.sublime-workspace"
  - vendor
  - .asset-cache
  - .bundle
  - .jekyll-assets-cache
  - .sass-cache
  - assets/js/plugins
  - assets/js/_main.js
  - assets/js/vendor
  - Capfile
  - CHANGELOG
  - config
  - Gemfile
  - Gruntfile.js
  - gulpfile.js
  - LICENSE
  - log
  - node_modules
  - package.json
  - package-lock.json
  - Rakefile
  - README
  - tmp
  - /docs # ignore Minimal Mistakes /docs
  - /test # ignore Minimal Mistakes /test
keep_files:
  - .git
  - .svn
encoding: "utf-8"
markdown_ext: "markdown,mkdown,mkdn,mkd,md"


# Conversion
markdown: kramdown
highlighter: rouge
lsi: false
excerpt_separator: "\n\n"
incremental: false


# Markdown Processing
kramdown:
  input: GFM
  hard_wrap: false
  auto_ids: true
  footnote_nr: 1
  entity_output: as_char
  toc_levels: 1..6
  smart_quotes: lsquo,rsquo,ldquo,rdquo
  enable_coderay: false


# Sass/SCSS
sass:
  sass_dir: _sass
  style: compressed # https://sass-lang.com/documentation/file.SASS_REFERENCE.html#output_style


# Outputting
permalink: /:categories/:title/
paginate: 5 # amount of posts to show
paginate_path: /page:num/
timezone: # https://en.wikipedia.org/wiki/List_of_tz_database_time_zones


# Plugins (previously gems:)
plugins:
  - jekyll-paginate
  - jekyll-sitemap
  - jekyll-gist
  - jekyll-feed
  - jekyll-include-cache

# mimic GitHub Pages with --safe
whitelist:
  - jekyll-paginate
  - jekyll-sitemap
  - jekyll-gist
  - jekyll-feed
  - jekyll-include-cache


# Archives
#  Type
#  - GitHub Pages compatible archive pages built with Liquid ~> type: liquid (default)
#  - Jekyll Archives plugin archive pages ~> type: jekyll-archives
#  Path (examples)
#  - Archive page should exist at path when using Liquid method or you can
#    expect broken links (especially with breadcrumbs enabled)
#  - <base_path>/tags/my-awesome-tag/index.html ~> path: /tags/
#  - <base_path>/categories/my-awesome-category/index.html ~> path: /categories/
#  - <base_path>/my-awesome-category/index.html ~> path: /
category_archive:
  type: liquid
  path: /categories/
tag_archive:
  type: liquid
  path: /tags/
# https://github.com/jekyll/jekyll-archives
# jekyll-archives:
#   enabled:
#     - categories
#     - tags
#   layouts:
#     category: archive-taxonomy
#     tag: archive-taxonomy
#   permalinks:
#     category: /categories/:name/
#     tag: /tags/:name/


# HTML Compression
# - https://jch.penibelst.de/
compress_html:
  clippings: all
  ignore:
    envs: development


# Defaults
defaults:
  # _posts
  - scope:
      path: ""
      type: posts
    values:
      layout: single
      author_profile: true
      read_time: true
      comments: # true
      share: true
      related: true

https://media.giphy.com/media/ClsZPj1jbbmcSTc942/giphy-downsized-large.gif

![image](https://giphy.com/gifs/ClsZPj1jbbmcSTc942/fullscreen);


![image](https://github.com/msirch/msirch.github.io/blob/main/iDrive_python.gif);

https://media.giphy.com/media/ClsZPj1jbbmcSTc942/giphy-downsized-large.gif
![my alternate text]([https://media.giphy.com/media/ClsZPj1jbbmcSTc942/giphy-downsized-large.gif](https://media.giphy.com/media/ClsZPj1jbbmcSTc942/giphy-downsized-large.gif));



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
