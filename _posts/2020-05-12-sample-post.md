---
layout: post
title: Sample Post
image: "/images/posts/25.png"
categories: [jekyll, docs]
---
Markdown (or Textile), Liquid, HTML & CSS go in. Static sites come out ready for deployment.

#### Headings

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

#### Blockquote

> No more databases, comment moderation, or pesky updates to install—just your content.

#### Unordered List

* Jekyll
    * Nested Jekyll
    * Nested Ruby
* Ruby
* Markdown
* Liquid

#### Ordered List

1. Jekyll
    1. Nested Jekyll
    2. Nested Ruby
2. Ruby
3. Markdown
4. Liquid

#### Link

This is <a href="http://example.com/" title="Title">an example</a> inline link.

#### Paragraph

Jekyll is a simple, blog-aware, static site generator. It takes a template directory containing raw text files in various formats, runs it through a converter (like Markdown) and our Liquid renderer, and spits out a complete, ready-to-publish static website suitable for serving with your favorite web server. Jekyll also happens to be the engine behind GitHub Pages, which means you can use Jekyll to host your project’s page, blog, or website from GitHub's servers for free.

### Quoting

> “Creativity is allowing yourself to make mistakes. Design is knowing which ones to keep.”

― Scott Adams
{: .cite}

#### Image
<figure class="aligncenter">
	<img src="https://images.unsplash.com/photo-1449452198679-05c7fd30f416?ixlib=rb-0.3.5&q=80&fm=jpg&crop=entropy&s=73181f1c6d56b933b30de2bfe21fdf3b" />
	<figcaption>Photo by <a href="https://unsplash.com/rmaedavis" target="_blank">Rachel Davis</a>.</figcaption>
</figure>

## Footnotes

The quick brown fox[^1] jumped over the lazy dog[^2].

[^1]: Foxes are red
[^2]: Dogs are usually not red

Footnotes are a great way to add additional contextual details when appropriate. Ghost will automatically add footnote content to the very end of your post.

## Tables

<table>
<caption>Table Caption</caption>
<thead>
<tr>
   <th>Content categories</th>
   <th>Flow content</th>
  </tr>
</thead>
 <tbody>
  <tr>
   <td>Permitted content</td>
   <td>
    An optional <code>&lt;caption&gt;</code> element;<br />
    zero or more <code>&lt;colgroup&gt;</code> elements;<br />
    an optional <code>&lt;thead&gt;</code> element;<br />
    an optional <code>&lt;tfoot&gt;</code> element;
   </td>
  </tr>
  <tr>
   <td>Tag omission</td>
   <td>None, both the start tag and the end tag are mandatory</td>
  </tr>
  <tr>
   <td>Permitted parent elements</td>
   <td>Any element that accepts flow content</td>
  </tr>
  <tr>
   <td>Normative document</td>
   <td><a href="http://www.whatwg.org/specs/web-apps/current-work/multipage/tabular-data.html#the-table-element" rel="external nofollow">HTML5, section 4.9.1</a> (<a href="http://www.w3.org/TR/REC-html40/struct/tables.html#edef-TABLE">HTML4.01, section 11.2.1</a>)</td>
  </tr>
 </tbody>
</table>

#### Default Code Block

    This is code blog.

#### Styled Code Block

    #!/usr/bin/ruby
    $LOAD_PATH << '.'
    require "support"

    class Decade
    include Week
       no_of_yrs=10
       def no_of_months
          puts Week::FIRST_DAY
          number=10*12
          puts number
       end
    end
    d1=Decade.new
    puts Week::FIRST_DAY
    Week.weeks_in_month
    Week.weeks_in_year
    d1.no_of_months


#### Bash code highlight
    sudo apt update
    sudo apt install asciidoc \
                     autoconf \
                     bc \
                     binutils-dev \
                     bison \
                     build-essential \
                     byobu \
                     fakeroot \
                     flex \
                     gawk \
                     git \
                     htop \
                     kernel-package \
                     kernel-wedge \
                     libattr1-dev \
                     libaudit-dev \
                     libbabeltrace-ctf-dev \
                     libbabeltrace-dev \
                     libblkid-dev \
                     libcap-dev \
                     libdevmapper-dev \
                     libdw-dev \
                     libelf-dev \
                     libiberty-dev \
                     liblzma-dev \
                     libncurses-dev \
                     libnuma-dev \
                     libperl-dev \
                     libselinux-dev \
                     libslang2-dev \
                     libssl-dev \
                     libtool \
                     libudev-dev \
                     libunwind-dev \
                     libzstd-dev \
                     linux-generic-hwe-18.04-edge \
                     python-dev \
                     python3-distutils \
                     rsync \
                     sysstat \
                     systemtap-sdt-dev \
                     time \
                     tmux \
                     unp \
                     uuid-dev \
                     zlib1g-dev

#### yaml code highlight
    registries:
      - username: gitlab+deploy-token-1
        password: $TOKEN
        registry_url: registry.some.url


Auto detect the language of the code and highlights the code, [More about highlight](https://highlightjs.org/static/demo/)

#### Definition Lists

<dl>
    <dt>Definition Title</dt>
    <dd>Definition Description</dd>
</dl>

### Image galleries

Here's a really neat custom feature we added – galleries:

<div class="gallery" data-columns="3">
  <img src="/images/demo/demo-portrait.jpg">
  <img src="/images/demo/demo-landscape.jpg">
  <img src="/images/demo/demo-square.jpg">
  <img src="/images/demo/demo-landscape-2.jpg">
</div>

Inspired by the Galleries feature from WordPress, we've made it easy to create grid layouts for your images. Just use a bit of simple HTML in your post to create a masonry grid image layout:

```html
<div class="gallery" data-columns="3">
    <img src="/images/demo/demo-portrait.jpg">
    <img src="/images/demo/demo-landscape.jpg">
    <img src="/images/demo/demo-square.jpg">
    <img src="/images/demo/demo-landscape-2.jpg">
</div>
```

*See what we did there? Code and syntax highlighting is built-in too!*

Change the number inside the 'columns' setting to create different types of gallery for all kinds of purposes. You can even click on each image to seamlessly enlarge it on the page.

### Image carousels

Here's another gallery with only one column, which creates a carousel slide-show instead.

A nice little feature: the carousel only advances when it is in view, so your visitors won't scroll down to find it half way through your images.

<div class="gallery" data-columns="1">
  <img src="/images/demo/demo-landscape.jpg">
  <img src="/images/demo/demo-landscape-2.jpg">
</div>

```html
<div class="gallery" data-columns="1">
  <img src="/images/demo/demo-landscape.jpg">
  <img src="/images/demo/demo-landscape-2.jpg">
</div>
```