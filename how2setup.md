## How to setup guide

* Install [Docker](https://docs.docker.com/engine/install/)
* `git clone https://github.com/xTent-robotics/xTent-robotics.github.io.git`
* Follow the [instructions](https://github.com/ashBabu/Utilities/wiki/Useful#jekyll-github-pages-using-docker) to get it up and
running in a browser
* Under `_data` edit the `navigation.yml` and `sitetext.yml` as required
* Under `_layouts`, `home.html` filters the ones that needs to be added to the website
* There is a `_config.yml` which if edited, need to be reloaded by `Ctrl+C` on terminal and rerun `docker run -p 4000:4000 -v $(pwd):/site jekyll-serve`
* To change the header image's properties, edit the [_masthead.scss](/_sass/layout/_masthead.scss_)

### Setting up the contact
* Go to [formspree](https://formspree.io/) and create an account
* Then [create a form](https://formspree.io/create). This will create something like `https://formspree.io/f/myuvkevb`
where the last part `f/myuvkevb` has to be added to the [config.yml](_config.yml) under the `formspree_form_path` tag