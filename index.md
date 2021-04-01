---
layout: default
title: Introduction
nav_order: 1
description: "Gmail Docs is a responsive Jekyll theme with built-in search that is easily customizable and hosted on GitHub Pages."
permalink: /
---

# Introduction

This document is for people who know the basic workings of sending and receiving emails through Gmail, but do not know how to use any of its lesser known features. Each section is a broad category that is split up into smaller features within.

Gmail is Google’s free to use email system that is available to every google account. This email system can be very powerful if used properly as it can be used with many other google products. This documentation will provide some instructions on some powerful functions, so they  can use Gmail to its fullest extent.

---

# Table of Contents

...

---

# Is This Guide For You

The guide is for beginner Gmail users who have basic sending and receiving email understanding. 

Everything discussed in this documentation will be for the Windows and Mac version of Gmail. Layouts and settings may differ if you are using iOS or Android. This guide will provide easy-to-understand instructions to understand and manipulate these features to your needs. By the end of this document you will be able to:

Automate emails/signature blocks
Effectively search for emails
Customize/personalize your Gmail
Use Add-ons/Built in google products
Create a safe environment for sending and receiving emails

---

# When It Is Written (Software version)
Web Version April 2021

---

# Prerequisite

The user must have a Google Account to access Gmail.

The user should use the latest version of Chrome, FireFox, Edge, and Safari. 
Note: IE11 is no longer to be supported.

---

# Brief History

Gmail is a free mail service that was released by Google on April 1, 2004, originally as an invitation-only email service. In addition to winning several awards, Forbes magazine also declared that it was the best webmail application for small business in 2006. Over the years, the user base and features have expanded greatly, reaching 1.5 billion active users in October 2019. 

Currently, it is a powerful tool that grants the user a high degree of customizability for their email needs. Integrations with Google’s other products such as Calendar, as well as third party add-ons grant every user a tailored experience. Its presence on mobile devices as an app also gives it great portability, especially as it’s the default mail app for android devices. 

---

# Why Learn Gmail

If you are a worker or businessman, you will need to send a lot of emails every day.
Therefore, learning how to customize and automate Gmail will help you to reduce workload.

---

# Typographical Convention

...

---

# Conclusion

Gmail’s extensive suite of features are often overlooked, thus making people think it is just a mediocre email system. However, Gmail is one of the most powerful email systems especially when used with other Google apps. 

With all this said, let us begin teaching these lesser known features. Creating Categories is a good place to start reading.

---

### ------------------------------

1. Install the Ruby Gem
```bash
$ gem install just-the-docs
```
```yaml
# .. or add it to your your Jekyll site’s Gemfile
gem "just-the-docs"
```
2. Add Just the Docs to your Jekyll site’s `_config.yml`
```yaml
theme: "just-the-docs"
```
3. _Optional:_ Initialize search data (creates `search-data.json`)
```bash
$ bundle exec just-the-docs rake search:init
```
3. Run you local Jekyll server
```bash
$ jekyll serve
```
```bash
# .. or if you're using a Gemfile (bundler)
$ bundle exec jekyll serve
```
4. Point your web browser to [http://localhost:4000](http://localhost:4000)

If you're hosting your site on GitHub Pages, [set up GitHub Pages and Jekyll locally](https://help.github.com/en/articles/setting-up-your-github-pages-site-locally-with-jekyll) so that you can more easily work in your development environment.

### Configure Just the Docs

- [See configuration options]({{ site.baseurl }}{% link docs/configuration.md %})

---

## About the project

Just the Docs is &copy; 2017-{{ "now" | date: "%Y" }} by [Patrick Marsceill](http://patrickmarsceill.com).

### License

Just the Docs is distributed by an [MIT license](https://github.com/pmarsceill/just-the-docs/tree/master/LICENSE.txt).

### Contributing

When contributing to this repository, please first discuss the change you wish to make via issue,
email, or any other method with the owners of this repository before making a change. Read more about becoming a contributor in [our GitHub repo](https://github.com/pmarsceill/just-the-docs#contributing).

#### Thank you to the contributors of Just the Docs!

<ul class="list-style-none">
{% for contributor in site.github.contributors %}
  <li class="d-inline-block mr-1">
     <a href="{{ contributor.html_url }}"><img src="{{ contributor.avatar_url }}" width="32" height="32" alt="{{ contributor.login }}"/></a>
  </li>
{% endfor %}
</ul>

### Code of Conduct

Just the Docs is committed to fostering a welcoming community.

[View our Code of Conduct](https://github.com/pmarsceill/just-the-docs/tree/master/CODE_OF_CONDUCT.md) on our GitHub repository.


[Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/pmarsceill/just-the-docs){: .btn .fs-5 .mb-4 .mb-md-0 }

{: .fs-6 .fw-300 }
{: .fs-9 }

Just the Docs is built for [Jekyll](https://jekyllrb.com), a static site generator. View the [quick start guide](https://jekyllrb.com/docs/) for more information. Just the Docs requires no special plugins and can run on GitHub Pages' standard Jekyll compiler. The [Jekyll SEO Tag plugin](https://github.com/jekyll/jekyll-seo-tag) is included by default (no need to run any special installation) to inject SEO and open graph metadata on docs pages. For information on how to configure SEO and open graph metadata visit the [Jekyll SEO Tag usage guide](https://jekyll.github.io/jekyll-seo-tag/usage/).
