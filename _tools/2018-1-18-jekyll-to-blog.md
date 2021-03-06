---
type: tools
title: 使用jekyll搭建博客
---

[Jekyll on Windows | jekyll](https://jekyllrb.com/docs/windows/)
提供了windows下的Ubuntu实现，方法简单，亲测成功。


- 写得很不错的：
  - [使用Github Pages建独立博客 | BeiYuu.com](http://beiyuu.com/github-pages)
  - [Jekyll搭建个人博客](http://baixin.io/2016/10/jekyll_tutorials1/)
  - [Build your own website (with Jekyll and Minimal-mistakes theme) - Li Zeng](https://zenglix.github.io/personal_website/)
  - [一碰minimal-mistakes就上手 - 我的後大學時代](https://kodeworker.github.io/%E6%95%99%E5%AD%B8/%E4%B8%80%E7%A2%B0minimal-mistakes%E5%B0%B1%E4%B8%8A%E6%89%8B/)

在这一步中，卡了好久：
- 设置：navigation.yml时，即设置不同的导航标签，类似这个：
关于navigation.yml中不同tab间的识别，还需要进一步学习。



### 其他
#### 数学公式 
- [Jekyll中使用MathJax](http://pkuwwt.github.io/linux/2013-12-03-jekyll-using-mathjax/)
不太起作用？
- [Kramdown does not seem to render math blocks · Issue #735 · mmistakes/minimal-mistakes](https://github.com/mmistakes/minimal-mistakes/issues/735)
mmistake作者解答：

1. 在/_includes/scripts.html
中加入：

```
{% if page.mathjax %}
<script type="text/javascript" async
  src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-MML-AM_CHTML">
</script>
{% endif %}
```

2. 在博客文章的yaml头部声明：
`mathjax: true`


## 多个导航栏记录不同内容。
- [Github Pages博客搭建过程记录 @ 技术杂货铺hjmao](https://huajianmao.github.io/how-i-setup-this-blog/)
- 基于jekyll的Collection实现。此方法可行，但是较复杂，推荐利用catagory实现。
  - [3 Simple steps to setup Jekyll Categories and Tags | Webjeda](https://blog.webjeda.com/jekyll-categories/)