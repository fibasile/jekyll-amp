# Jekyll-amp Documentation

Jekyll-amp  is a jekyll theme suitable for [AMP](https://www.ampproject.org/) Accelerated Mobile Pages.

The idea is to have a Jekyll-powered scaffold ready to be used for a new project, with all the work needed to include AMP functionality already done.

See also the [ROADMAP](./ROADMAP.md) and [Contribution Guidelines](./CONTIBUTING.md).


# Getting started

You can start by cloning the Github repo, available at:

[https://github.com/fibasile/jekyll-amp](https://github.com/fibasile/jekyll-amp)

If you are on a MacOS or Linux system, just run the following to start development:

```bash
$ git clone https://github.com/fibasile/jekyll-amp.git
$ cd jekyll-amp
$ bundle
$ jekyll serve
```

Since Jekyll-AMP runs standard Jekyll, you can use the [Jekyll](http://jekyllrb.org) doumentation as a reference on customization, plugins and publishing workflow.

The following sections descibe the AMP specific features.


# AMP modules

## Images

## Articles

## Galleries

## Embedding content from social networks

You can embed a number of content types using one of the many available AMP modules.

- Twitter posts
- Instagram posts
- Instagram stories
- Youtube videos
- Vimeo videos
- Facebook Posts
- Facebook stories
- Facebook pages

# Configuration

In the `_config.yml` file you find the standard Jekyll config, plus some additional settings for the theme.

The **amp_modules**  key defines all the AMP modules enabled, you can comment or uncomment lines based on the modules you are using. Modules are grouped into different categories:

```yaml
amp_modules:
 embed:
    twitter:
    instagram:
    youtube:
    facebook:
```

# Customization

## Base layout

The base layout is based on the AMP skeleton, including ...

## Stylesheets

AMP specification requires pages contain a single stylesheet or inline styles. With Jekyll this is not a real problem, since we can use the include mechanism on a per page basis to include custom styles for each page.

The base stylesheet is contained inside the `_includes/default_style.css`.

Defining the `include_style` variable in a layout or page front-matter, allows you to add another custom css include to each page. Specify the filename including extension and place your file inside the `_includes` folder.