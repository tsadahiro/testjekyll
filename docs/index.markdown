---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

ターミナル・シェルの利用について基本を解説致します。

* 「システム運用」等の授業で必要となる。
* IOT機器、ネットワーク上のサーバの操作などで必要となる。

というのが、主な理由ですが、普段のPC利用においても
役に立つことが多いと考えるからです。

系統だった詳細な説明とはならないかも知れませんが、
私が経験上よく使う、または有効だと思える機能に
ついて説明します。

<ol>
  {% for item in site.data.lessons %}
	<li>
    <a href="lessons/{{ item.link }}" 
	{% if page.url == item.link %}style="color: red;"{% endif %}>
	{{ item.num }}
    </a>
	</li>
  {% endfor %}
</ol>
