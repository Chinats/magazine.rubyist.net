---
layout: default
title: るびま
---
{% include base.html %}

## Rubyist Magazine について

『Rubyist Magazine』、略して『るびま』は、日本 Ruby の会の有志による Rubyist の Rubyist による、Rubyist とそうでない人のためのウェブ雑誌です。

## 最新号

{% for post in site.tags.index limit: 1 %}
<div class="card">
    <h5 class="card-header">
      <a href="{{base}}{{ post.url }}">{{post.title}}</a>
    </h5>
    <div class="card-body">
      {{post.description}}
    </div>
</div>
{% endfor %}

## バックナンバー

<div class="card-group">
{% for post in site.tags.index limit: 5 %}
    <div class="card">
        <h5 class="card-header">
            <a href="{{base}}{{ post.url }}">{{post.title}}</a>
        </h5>
        <div class="card-body">
            {{post.description}}
        </div>
    </div>
{% endfor %}
</div>

<a href="#">さらに過去のバックナンバー</a>

## FAQ

### 一般

- Q. るびま、って「ネギま！」のぱくりですか？
- A. 違います。多分。「るびま」を考えた人たちは「ネギま！」を知りませんでした (または、言われるまで気付かなかった)。

- Q. 日本 Ruby の会って、るびまを発行することを目的とする団体ですか？
- A. 違います。るびまは、日本 Ruby の会の活動の一環として日本 Ruby の会有志によって編集作業が行われています。

- Q. 日本 Ruby の会発足とるびま創刊号発行は同時なの？（CNET の記事より）
- A. 違います。発足は 2004 8/8, 創刊号の発行は 2004 9/10 です。

- Q. 何が嬉しくてやってんの？
- A. 執筆者、編集者によります。営利目的じゃありません。

- Q. 月刊なんですか？
- A. 違います。

- Q. じゃぁ、何時出すんですか？
- A. 出せそうだと思ったら出します。

- Q. るびまに宣伝を出したいんだけれど。
- A. 可能です。詳しくは るびま編集部 までご連絡ください。

- Q. るびまの読者プレゼントに提供したいものがあるんだけれど。
- A. 歓迎します。るびま編集部 までご連絡ください。

- Q. 問い合わせはどこにすればいいの？
- A. るびま編集部 にお願いします。
