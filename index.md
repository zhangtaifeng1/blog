---
layout: home
---

<div class="index-content home">
    <div class="section">
        <ul class="artical-cate">
            <li class="on"><a href="/"><span>Home</span></a></li>
            <li style="text-align:center"><a href="/opinion"><span>Opinion</span></a></li>
            <li style="text-align:right"><a href="/project"><span>Project</span></a></li>
        </ul>

        <div class="cate-bar"><span id="cateBar"></span></div>

        <ul class="artical-list">
        {% for post in site.categories.home %}
            <li>
                <h2>
                    <a href="{{ post.url }}">{{ post.title }}</a>
                    <small class="post-time">{{ post.date|date:"%Y-%m-%d" }}</small>
                </h2>
                <div class="title-desc">{{ post.description }}</div>
            </li>
        {% endfor %}
        </ul>
    </div>
    <div class="aside">
    </div>
</div>

