# OpenData-Backbone

A sample application demonstrating how an application might be built against the Open Data API using Backbone.js and Marionette.js.

# Prerequisites
1. [nodejs and npm](http://nodejs.org/)
1. [bower](http://bower.io/) (`npm install -g bower`)
1. [phantomjs](http://phantomjs.org/) (for tests)

# Setup
1. Clone the repo: `git clone git@github.com:mjuniper/OpenData-Backbone.git`
2. `cd OpenData-Backbone`
2. `npm install`
3. `bower install`
4. `gulp serve`

# S3 Deployment
0. Follow setup instructions
0. Create S3 Bucket
  * Enable Website Hosting
  * Set default index document to `index.html`
  * Set default error docuement to `404.html`
0. `cp gulp-aws.json.example gulp.aws.json`
0. Fill in AWS credentials
0. Fill in bucket name
0. `gulp publish`
0. Visit S3 Website host

# Roadmap
Not a roadmap in the sense that these are features that will *definitely* be implemented; more of a list of potential improvements

* API v2
* upgrade yuki
* leaflet mapmanager with config flag (if we go this route, the mapmanager should load it's own dependencies)
* more tests
