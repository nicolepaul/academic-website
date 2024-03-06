---
title: How did I make my personal academic website?
summary: '*A simple and free to low-cost way to create a personal academic website for those with some basic comfort using code and Git.*'
date: 2024-03-05
math: true
toc: true
image:
  placement: 2
  caption: ''
tags:
- academia
- website
---

## Introduction

[Establishing an online presence as an academic](https://www.jackwbaker.com/advice/Online_presence.html) can help others learn more about your research and serve as an online CV for future career opportunities.

This guide shares the steps to create a website similar to mine. It is meant for those that have some comfort with coding and Git. There are a variety of alternative options that do _not_ require coding or the use of Git, such as [Google Sites](https://sites.google.com/), [Squarespace](https://www.squarespace.com/), or [Wix](https://www.wix.com/). Additionally, your university may support creation of a personal page on their website.

Personally, I chose [Hugo](https://gohugo.io/) because I wanted to maintain my website in a text editor rather than by clicking around on a browser. I felt this would maximize my degree of control, while still allowing me to take advantage of pre-built web components and themes. Ultimately, you should choose whichever option makes sense for you, both in terms of the initial setup and longer-term maintenance. To deploy my static website, I'm using [Netlify](https://www.netlify.com/), which is free for my use case. Lastly, I manage my domain name using [Cloudflare](https://www.cloudflare.com/).

In terms of costs for this website, I only pay for the domain name: 45USD annually (3.75USD monthly). However, several cheaper alternative domain names were available (e.g., 10USD annually) and free domain names are possible with Netlify or GitHub Pages.

## Building your website

### Hugo: Static site generator

Before I made my website, I sifted through other academics' websites to get a feel for what I liked and which options had my desired functionality or look/feel. I saw that many academics used [Hugo](https://gohugo.io/), an open source static site generator. You can learn more about Hugo [here](https://gohugo.io/about/what-is-hugo/).

After some initial orientation, Hugo is relatively simple to use and customize without having to get into the weeds of dependencies, databases, and so on. The result is a website that is fast and customizable.

### Choosing a theme

Hugo has a variety of themes for different purposes, from personal academic CVs to research lab pages and portfolios to books. You can see the full list of themes [here](https://themes.gohugo.io/). The right theme for you may depend on what type of content you want to showcase. 

For this website, I'm using the [Academic CV](https://hugoblox.com/templates/details/academic-cv/) theme, which is free. However, I've customized the styling quite a bit to make the website feel a bit more personalized. 


### Configuring settings

Go through the files in the `config/` folder to set your website settings. In general, you can use the defaults. However, some important settings to configure include:
* Website title (`title`)
* Base URL (`baseURL`) -- *do this once you've chosen a domain name*
* Menu order
* Appearance (e.g., `mode`, `theme`, `font`, `font_size`)
* Search engine optimization (SEO) and marketing (`seo`, `marketing`) -- *note that it can take a day or two for your website to appear on search engines*

### Adding content

Once you've identified the theme you'd like to work with, follow the edit/download link. This should take you to the Github repository for the code, which you can fork (copy) and edit in your preferred text editor (e.g., [VSCode](https://code.visualstudio.com/)).

In general, all of the content is within markdown files inside the `content/` folder.

#### Landing page

The main landing page is at the path: `content/_index.md`. Here, you can choose the order of your content, remove sections, and choose between different [views](https://docs.hugoblox.com/getting-started/page-builder/#personalizing-blocks) for the content.

#### Content types

There should already be dummy examples of the different content types (e.g., projects, blog posts, biography) that you can adapt as needed. Refer to the [Hugo Blox Docs](https://docs.hugoblox.com/reference/markdown/) for more infortmation on how to customize your content.

Different content types support different parameters, which are specfiied at the top of each markdown file between lines of `---`. The main body is specified after the parameters, using general Markdown syntax. For reference, a simple example is shown for a project below.

```yaml
---
# Parameters: General information
title: An example project
summary: Here is a brief summary of the example project
tags:
  - academia
  - website
date: '2019-11-01T00:00:00Z'
show_date: False
# Parameters: Optional links that will appear as badges
links:
url_code: 'https://github.com/nicolepaul'
url_pdf: ''
url_slides: ''
url_video: 'https://youtube.com/'
---
<!--- The content below will go into the main body of the page -->
## Overview

Some text here.

## Acknowledgments

Some text here.
```

### Custom styling

Some ways you can customize the styling of your selected theme include:
* Adding an icon (favicon)
* Setting a color theme
* Choosing fonts
* Adjusting the navigation bar
* Changing the order of content in the menus

Refer to the [Hugo Blox Docs](https://docs.hugoblox.com/getting-started/customize/) for the supported customization options.

For more advanced styling, you can always add your own custom css at the following path: `assets/scss/custom.scss`. This will override the default styling.

## Deploying your website

### Deploying locally

In order to deploy locally, you will first need to follow the [Hugo installation guidelines for your machine type](https://gohugo.io/installation/). I recommend doing this so that you can preview your changes and check for any errors before updating your repository's `main` branch and affecting the production version deployed online.

After you've installed Hugo and its dependencies, you can deploy locally from a terminal window. First, navigate to your repository's root directory. From there, you can call `hugo server` to deploy locally. A message should appear with an address you can navigate to on your browser (e.g., `http://localhost:1313/`).

You can also view live changes when you deploy locally. That means, you can edit the files and the instantly see changes in your browser.

### Deploying online

Hugo websites can be deployed by a [variety of services](https://docs.hugoblox.com/reference/deployment/).

#### Netlify

[Netlify](https://www.netlify.com/) is free and easy to use, and will automatically update when you commit changes to your repository's `main` branch.

To do this, link your Netlify account to your Github account and find the repository hosting the code for your personal website. Once an update to the `main` branch of your repository is detected, it should only take a minute or two for Netlify to build and deploy the latest changes.

#### GitHub Pages

GitHub also lets you host a static site for free. To do so, you need the code repository to be named `<USERNAME>.github.io`. Detailed guidance on how to set up a Hugo website using GitHub Pages is available [here](https://www.o11ycloud.com/posts/gh_hugo/).

## Domain names

There are free and paid options for your domain name. Once you decide, don't forget to update the `baseURL` parameter in the relevant file in the `_config/` folder!

### Finding a domain name

If you want, you can use a free doamin name from Netlify (`<NAME_HERE>.netlify.app`) or GitHub Pages (`<USERNAME>.github.io`).

However, you can also purchase your own domain name from a variety of providers. You can search for available domain names and prices on services such as [Hover](https://www.hover.com/) or [Namecheap](https://www.namecheap.com/). Pay attention to any listed renewal costs, which are sometimes higher than the initially listed price.

### Setting up a DNS record

{{% callout note %}}
The **Domain Name System (DNS)** acts as a phonebook of the internet. The DNS maps human-friendly domain names or hostnames (e.g, example.com) to computer-friendly Internet Protocol (IP) addresses (e.g., 192.0.2.1).
{{% /callout %}}

Once you have a domain, you need to add a DNS record in whichever service you use to manage your domain (e.g., Cloudflare). Netlify provides [several guides to help you configure your DNS settings](https://answers.netlify.com/t/support-guide-compiled-resources-for-production-domains-on-netlify-and-dns-settings-start-here/48222), as does [GitHub Pages](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

Note that it can take between a few minutes to three days for your DNS record to be propagated (i.e., to correctly direct to your website).