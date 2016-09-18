WBlog
=======
[![Build Status](https://travis-ci.org/victorialice/AliceBlog.svg?branch=master)](https://travis-ci.org/victorialice/AliceBlog)
[![Code Climate](https://codeclimate.com/github/victorialice/AliceBlog.png)](https://codeclimate.com/github/victorialice/AliceBlog)
[![Test Coverage](https://codeclimate.com/github/victorialice/AliceBlog/coverage.png)](https://codeclimate.com/github/victorialice/AliceBlog)

The missing open source blog system on Ruby on Rails.

WBlog is open source blog which built for mobile first, it's licenced on MIT, use it for free!

[中文说明文档](/README.zh-CN.md)

Characteristic:

* Modern clean reading feelings
* Markdown support, give nice formatted articles
* Mobile first, responsive page for iPhone, iPad, iMac.
* Independent comment system, subscribe system, picture manage system

A demo came from my English blog: <http://en.zhuwenqian.com>

Another demo using my blog: <http://zhuwenqian.com>

Power Admin Dashboard: <http://en.zhuwenqian.com/admin>, user and password are configurable.

Some [screenshots](#screenshots)

### System dependencies

* Ruby ( = 2.3.1 )
* Postgresql ( >= 9.x )
* Nginx ( >= 1.4 )

### Features

* Responsive, iPhone, iPad, Notebook, PC, all are supported
* QR Code, Like button make your article easily sharing with your friends
* Inpendent comment system, subscribe system, that all belong to you
* Markdown supported, code highlight, especially for programmer, like you
* Personalize it, commercialize it, it all depends on you

### Goal

Make it to the best Ruby on Rails Blog system in the world.

### Running in development mode

WBlog MUST run in Linux or OSX. I assume you are using OS X 10.

You can run it like a Ruby on Rails project as usual:

0. Check dependencies

  ```shell
  ruby -v
  # 2.3.1
  postgres  --version
  # 9.x.x
  ```

1. Clone it

  `git clone git@github.com:victorialice/AliceBlog.git`

  `cd AliceBlog`

2. Install dependencies & configure

  ```shell
  gem install bundler
  bundle install
  cp config/application.yml.example config/application.yml
  cp config/database.yml.example config/database.yml
  ```

  Update `application.yml` & `database.yml` 's content as you need

3. Start it

  ```shell
  rails s
  ```

  Open browser with `http://localhost:3000`

  If there is any error found, please check your database's user and password.

4. Post the first blog

  visit: http://localhost:3000/admin, input your username and password configurated in `application.yml`.
  then, post a new article.

OK, That's all.

### Deployment

WBlog uses `mina` as automation deployment tool, uses `unicorn` as the Rack container.

WBlog recommends `nginx` as reverse proxy server.

It will be very fast.

Ruby on Rails project deployment is another topic, I would NOT talk it here.

You can read WBlog wiki for more information: [WBlog 的发布流程(Chinese only now)](https://github.com/victorialice/AliceBlog/wiki)

### Stack

* Ruby on Rails 5.0.0
* Ruby 2.3.1
* Turbolinks / SJR
* Foundation 6
* mina
* slim
* Postgresql


## Related open source blog systems

* writings.io( Ruby on Rails 4.0.2 ): a multi users blog system <https://github.com/chloerei/writings>
* jekyll( Ruby Gem, Markdown): Static blog system <http://jekyllrb.com/>
* octopress( Github Pages ): <http://octopress.org/>
* middleman( Ruby Gem ): Another static blog system <https://github.com/middleman/middleman>
* robbin_site( Padrino ): <https://github.com/robbin/robbin_site>

## License

MIT.

### Screenshots

Home Page:

![screenshot home](https://github.com/victorialice/AliceBlog/raw/master/doc/AliceBlog_s_en/home.png)

Home Page for mobile:

![screenshot home small](https://github.com/victorialice/AliceBlog/raw/master/doc/AliceBlog_s_en/home-small.png)

Home Page Hover Status for mobile:

![screenshot home hover](https://github.com/victorialice/AliceBlog/raw/master/doc/AliceBlog_s_en/home-small-hover.png)

Blog Show Page:

![screenshot post](https://github.com/victorialice/AliceBlog/raw/master/doc/AliceBlog_s_en/post.png)

Blog Show Page Hover Status:

![screenshot post hover](https://github.com/victorialice/AliceBlog/raw/master/doc/AliceBlog_s_en/post-hover.png)

Admin Login Page:

![screenshot admin](https://github.com/victorialice/AliceBlog/raw/master/doc/AliceBlog_s_en/admin-login.png)

Admin Dashboard Page:

![screenshot admin](https://github.com/victorialice/AliceBlog/raw/master/doc/AliceBlog_s_en/admin-dashboard.png)

Admin New Blog Page:

![screenshot admin](https://github.com/victorialice/AliceBlog/raw/master/doc/AliceBlog_s_en/admin-post.png)

Admin Blogs Manage Page:

![screenshot admin](https://github.com/victorialice/AliceBlog/raw/master/doc/AliceBlog_s_en/admin-posts.png)