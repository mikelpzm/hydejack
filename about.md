---
layout: about
title: About
description: >
  **Hydejack** is a Jekyll theme with JavaScript powers, combining the best of static sites and modern web apps.
  It features a suite of JavaScript that makes the page feel like an app, without sacrificing backwards-compatibility,
  page-load speed or SEO.
menu: true
order: 4
---

**Hydejack** aims to be the complete package for professionals on the web.
It features a blog suitable for both prose and technical documentation,
a showcase for your projects, and a resume that fits with the rest of the design.

> Your presence on the web --- A [blog], a [portfolio] and a [resume].
{:.lead}

## Download
There are two versions of **Hydejack**: The *free version* includes basic blogging functionality,
as did previous versions of the theme.
The *PRO version* includes additional features for professionals:
A [portfolio], a [resume] layout and a [welcome] page to feature your favorite projects and posts.

This table details what is and isn't included in each respective version.

|                                     | Free               | PRO                |
|:------------------------------------|:------------------:|:------------------:|
| Blog                                | &#x2714;           | &#x2714;           |
| [Features][feat]                    | &#x2714;           | &#x2714;           |
| [Portfolio] Layout                  |                    | &#x2714;           |
| [Resume] Layout                     |                    | &#x2714;           |
| [Welcome] Layout                    |                    | &#x2714;           |
| [Newsletter Box][news]              |                    | &#x2714;           |
| [Custom Forms][forms]               |                    | &#x2714;           |
| License                             | [GPL-3.0][license] | [PRO]              |
| Price                               | Free               | $29                |
|| [Download on GitHub][github]<br/> – or – <br/>[Use the RubyGem][gem] | [Buy Now][buy] [^1] |
{:.stretch-table}

## Features
Both versions include *all* of these features:

* Full in-app page loading, powered by [hy-push-state]{:.external}
* A customizable sidebar that turns into a drawer menu on mobile, powered by [hy-drawer]{:.external}
* Advanced FLIP animations, inspired by Material Design
* Good [Google PageSpeed Score][gpss][^2]
* Higher *perceived speed* thanks to content pre-fetching
* [Syntax highlighting](#syntax-highlighting), powered by [Rouge]
* [LaTeX math blocks](#latex-math-blocks), powered by [KaTeX]
* Change the wording of built-in strings and possibly translate in other languages
* Support for categories and tags
* Built-in icons for many social networks
* Simple and semantic HTML — can be viewed even with text-based browsers
* Author section below each article and support for multiple authors
* Progressive enhancement — sacrifice features, not content
* Google Analytics and Google Fonts support
* Disqus comments
* Print layout — Used to render Hydejack's [PDF documentation][pdf]
* Blog layout via `jekyll-paginate` (optional)
* SEO meta tags via `jekyll-seo-tag` (optional)
* Github avatars via `jekyll-avatar` (optional)
* Gist support via `jekyll-gist` (optional)

### Syntax Highlighting
Syntax highlighting powered by [Rouge].

~~~js
// Example can be run directly in your JavaScript console

// Create a function that takes two arguments and returns the sum of those
// arguments
var adder = new Function("a", "b", "return a + b");

// Call the function
adder(2, 6);
// > 8
~~~

### LaTeX Math Blocks
Write formulas in familiar LaTeX syntax. Powered by [KaTeX].

$$
\begin{aligned}
  \phi(x,y) &= \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right) \\[2em]
            &= \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j)            \\[2em]
            &= (x_1, \ldots, x_n)
               \left(\begin{array}{ccc}
                 \phi(e_1, e_1)  & \cdots & \phi(e_1, e_n) \\
                 \vdots          & \ddots & \vdots         \\
                 \phi(e_n, e_1)  & \cdots & \phi(e_n, e_n)
               \end{array}\right)
               \left(\begin{array}{c}
                 y_1    \\
                 \vdots \\
                 y_n
               \end{array}\right)
\end{aligned}
$$

### Customizable
**Hydejack** can be customized in a variety of ways, using only the `_config.yml` file.

```yml
# The string encoding which fonts to fetch from Google Fonts.
# See <https://qwtel.com/hydejack/docs/configuration/>
google_fonts:          Roboto+Slab:700|Noto+Sans:400,400i,700,700i

# The text font. Expects a string that is a valid CSS font-family value.
font:                  "'Noto Sans', Helvetica, Arial, sans-serif"

# The font used for headings. Expects a string that is a valid CSS font-family value.
font_heading:          "'Roboto Slab', Helvetica, Arial, sans-serif"

# Fallback image and color
accent_image:          /hydejack/assets/img/sidebar-bg.jpg
accent_color:          '#4fb1ba'
```

Check out the [full annotated `_config.yml` file](https://github.com/qwtel/hydejack/blob/master/_config.yml) for more.

You can change the wording of all built-in strings and labels by editing `strings.yml`.

```yml
---
  home:                Home
  pages:               Pages
  posts:               Posts
  about:               About
  related_posts:       Related Posts
  other_projects:      Other Projects
  comments:            Comments
  jump_to:             Jump to
  navigation:          Navigation
  social:              Social
  links:               Links
  pagination:          Pagination
  newer:               Newer
  older:               Older
  back:                Back
```

Check out the [full `strings.yml` file](https://github.com/qwtel/hydejack/blob/master/_data/strings.yml) for more.

## Versions
### Free Version
The *free version* features the design and tech of **Hydejack**, but only supports basic blogging.

[Download on GitHub][github] – or – [Use the RubyGem][gem]

### PRO Version
The *PRO version* aims to be the complete package for professionals on the web.
It includes layouts for your [portfolio],
your [resume] (with support for [JSON Resume](https://jsonresume.org/)),
a [welcome] page to introduce yourself to visitors,
built-in support for [Tinyletter], and from element styles so you can build arbitrary contact forms.

[Buy Now - $29][buy] [^1]

[^1]: Transactions secured by [Stripe](https://stripe.com). Downloads handled by [Simple Goods](https://simplegoods.co/).  
[^2]: Actual page load speed depends on your hosting provider, resolution of embedded images and usage of 3rd party plugins.  

[blog]: https://qwtel.com/hydejack/blog/
[portfolio]: https://qwtel.com/hydejack/projects/
[resume]: https://qwtel.com/hydejack/resume/
[download]: https://qwtel.com/download/
[welcome]: https://qwtel.com/hydejack/
[forms]: https://qwtel.com/hydejack/docs/7.1.1/forms-by-example/

[feat]: https://qwtel.com/hydejack/#features
[news]: https://qwtel.com/hydejack/#newsletter-subscription-box
[syntax]: https://qwtel.com/hydejack/#syntax-highlighting
[latex]: https://qwtel.com/hydejack/#latex-math-blocks

[license]: LICENSE.md
[pro]: licenses/PRO.md
[docs]: docs/7.1.1/index.md

[github]: https://github.com/qwtel/hydejack/releases
[gem]: https://rubygems.org/gems/jekyll-theme-hydejack
[buy]: https://app.simplegoods.co/i/AQTTVBOE

[gpss]: https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fqwtel.com%2Fhydejack%2F
[wiki]: https://github.com/qwtel/hydejack/blob/master/docs/7.1.1/index.md
[pdf]: https://github.com/qwtel/hydejack/releases/download/v7.1.1/Documentation._.Hydejack.pdf
[hy-push-state]: https://qwtel.com/hy-push-state/
[hy-drawer]: https://qwtel.com/hy-drawer/
[rouge]: http://rouge.jneen.net
[katex]: https://khan.github.io/KaTeX/
[tinyletter]: https://tinyletter.com/

*[FLIP]: First-Last-Invert-Play. A coding technique to achieve performant page transition animations.
