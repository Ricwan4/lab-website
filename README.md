# AND Lab Website

[![Twitter URL](https://img.shields.io/twitter/url?label=%40ANDlab3&style=social&url=https%3A%2F%2Ftwitter.com%2FANDlab3)](https://twitter.com/ANDlab3)

**[Affective, Neuroscience and Decision-making Lab](https://www.andlab-um.com)** is part of [CCBS](https://ccbs.ici.um.edu.mo) at [University of Macau](https://um.edu.mo).

This website is built with [Jekyll](https://jekyllrb.com/). It is derived from the great template provided by [research-lab-website](https://github.com/ericdaat/research-lab-website) and [Allan Lab](https://www.allanlab.org/aboutwebsite.html), at Leiden University.
## Local Setup & Run

Install Ruby firstly, then install Jekyll.

``` bash
gem install bundler jekyll
```

Clone this repository, then install the dependencies:

``` bash
git clone https://github.com/andlab-um/lab-website.git
cd lab-website
bundle install
```

Deploy the website locally with:

``` bash
bundle exec jekyll serve
```

## Contribute

### Add a new member

Adding new member photos under [assets/images/team](assets/images/team/) folder. Member information are stored as yaml file under [_data/member.yml](_data/member.yml). Each entry must look like this (**be careful with spaces**):

> It's better to learn some basic rules of yaml, like [YAML tutorial in the context of Jekyll](https://idratherbewriting.com/documentation-theme-jekyll/mydoc_yaml_tutorial). Some items are not necessary. The optimal personal photo width-height ratio is 3:4.

``` yaml
- title: Role of following members
  members:
    - name: Member name
      image: Member image file name
      content: Some description
      social:
        email: Email address
        website: Personal website
```

### Add a new publication

Publications are stored as markdown file under
[_pages/publication.md](_pages/publication.md). Just add a new entry like this (check [basic markdown syntax](https://www.markdownguide.org/basic-syntax)):

``` markdown
Wu, H., Fung, B. J., & Mobbs, D. (2022). **Mentalizing during social interaction: the development and validation of the interactive mentalizing questionnaire**. *Frontiers in psychology*, 12. [[Link](https://doi.org/10.3389/fpsyg.2021.791835){:target='_blank'}]
```

> Update (2022-12-07): please also add a BibTex entry at the beginning of the [assets/files/ANDlab-publications-Bibtex.bib](assets/files/ANDlab-publications-Bibtex.bib) file.

### Add news

Just post it on our lab Twitter account and it will automatically show up.

### Edit template

We use [Bootstrap v3](https://getbootstrap.com/) for designing the website. Feel free to modify either the [_pages](_pages/) or the
[_layouts](_layouts/) components.
