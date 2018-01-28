---
layout: post
title: Blogging on github and jekyll
category: hack
tags: github, jekyll
keywords: github, jekyll
---
# use the fxxxing google
* read  [使用 GitHub 免費製作個人網站](https://gitbook.tw/chapters/github/using-github-pages.html)
*  fork this site  [yansu]{https://github.com/suyan/suyan.github.io}
* gemfile is improtant

```
source 'https://rubygems.org'
gem 'github-pages'
gem 'jekyll-paginate'
gem 'jekyll-sitemap'
gem 'jekyll-admin', group: :jekyll_plugins
```
# recording
## install
- 到local github目錄，terminal 下　jekyll new afenc.github.io
- 然後將theme clone到該目錄 new afenc.github.io (但是gemfile要小心，這個設定這重要，需要備分一下)

```
group :jekyll_plugins do
gem "jekyll-paginate"
gem "jekyll-sitemap"
gem "jekyll-admin"
end
```

- 安裝好需要的jekyll plugins
- 總是要讓server跑起來(bundle exec jekyll serve)，才能在	http://localhost:4000/  測試
- admin目前需要手動加meta data像是tag, layout，不如直接在atom中duplicate舊的post就好。
- yansu的模版會自已分類
- avatar有點難找，就用find找sidebar.html之類的地方；需放在[圖床](https://i.imgur.com/2WaoXT8.jpg)
- [Jekyll及GitHub教學1》快速20分鐘建立免費部落格](http://hungchicheng.me/2017/05/11/how-to-make-blog-on-github/)
- [Jekyll及GitHub教學2》更換主題及安裝插件](http://hungchicheng.me/2017/05/13/how-to-make-jekyll-plugin/)
- [admin](https://github.com/jekyll/jekyll-admin)
Start Jekyll as you would normally (bundle exec jekyll serve)
Navigate to http://localhost:4000/admin to access the administrative interface
- [使用 Jekyll 建立自己的 Github Page Blog](https://nk910216.github.io/2017/02/05/HowToSetupBlog/)
- [使用 GitHub 免費製作個人網站](https://gitbook.tw/chapters/github/using-github-pages.html)
- 有固定page放在
```
"a href="/pages/xxx.html"
```
