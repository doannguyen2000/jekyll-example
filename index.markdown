---
layout: default
---
<div class="row">
    <div class="col">
        <div class="jumbotron p-4">
            <h1 class="display-4">Chào mừng đến với Jekyll!</h1>
            <p class="lead">Jekyll công cụ mạnh mẽ giúp bạn xây dựng Website / Blog HTML tĩnh.</p>
            <hr class="my-4">
            <p>Đây là trang ví dụ được xây dựng từ Jekyll với bài hướng dẫn chi tiết.</p>
            <a class="btn btn-primary btn-lg" href="https://xuanthulab.net" role="button">Xem thêm</a>
        </div>
    </div>
</div>
<div class="card m-4">
    <div class="card-header">
        Các bài viết
    </div>
    <div class="list-group list-group-flush">
        {% for post in site.posts %} 
            <a class="list-group-item list-group-item-action" href="{{ post.url | relative_url }}">{{ post.title }}</a>
        {% endfor %}
    </div>
</div>