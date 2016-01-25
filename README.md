ngn-colorado.github.io
======================

Our website is using [Jekyll](http://jekyllrb.com) -- a static page generator that is well integrated with Github pages. As opposed
to full blog platforms, Jekyll simply generates static HTML files from a combination of template and markup files.

Editing Content
---------------
All pages are located in `/pages` and are simple markdown files. `/data` contains all files that are being referenced from the pages.
Simply modify the Markdown document to change a page's content.

Building the Site
-----------------
When pushing the repository to Github, the static files are automatically built and published. However, the site can also be built
and viewed locally before pushing (and thereby publishing) changes. Jekyll requires Ruby and is bundled in the Gemfile in the
repository's main directory. In order to setup Jekyll (assuming you have Ruby (> 2.0) installed), execute the following steps:

	$ gem install bundler
	$ bundle install
  
Jekyll should now be installed. You can now either

	$ bundle exec jekyll build
  
to build the website in the `_site` directory, or 

	$ bundle exec jekyll serve
  
to start up a webserver listening on port 4000 which is serving the built site.

