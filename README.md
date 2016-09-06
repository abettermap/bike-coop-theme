# bike-coop-theme

## About

We are rebuilding the Fort Collins Bike Coop website currently. Our objective is to make it mobile friendly and add in a form to enable users to submit Volunteer Applications and Report Stolen Bikes.

This repository focuses on Theme development, related project repositories can be found here:

- [The central repository for the project is located here.](https://github.com/CodeForFoco/bike-coop)
- [The code for the project theme is located here.](https://github.com/CodeForFoco/bike-coop-plugin)
- [The code for the project plugin is located here.](https://github.com/CodeForFoco/bike-coop-theme)


## Contributing

We welcome new contributors. Not sure where to start? Check for any [open issues ](https://github.com/CodeForFoco/bike-coop/issues) or ping the team on [our slack channel](https://codeforfoco.slack.com/).

Ensure your code follows best practices and adheres to good style.

Contribution Workflow:

1. [Fork](https://help.github.com/articles/fork-a-repo/) this repository and clone your fork.
1. Make any changes, commit and push.
1. Submit a pull request and your changes will be reviewed and merged.

If you are unfamiliar with git, check the resources below or ping us on Slack and we'll help you out.

### Git

- [Fork A Repo](https://help.github.com/articles/fork-a-repo/)
- [Github Workflow](https://guides.github.com/introduction/flow/)

# Original Foundation Repo README [![Build Status](https://travis-ci.org/olefredrik/FoundationPress.svg?branch=master)](https://travis-ci.org/olefredrik/FoundationPress)
[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/olefredrik/foundationpress?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

This is a starter-theme for WordPress based on Foundation 6, the most advanced responsive (mobile-first) framework in the world. The purpose of FoundationPress, is to act as a small and handy toolbox that contains the essentials needed to build any design. FoundationPress is meant to be a starting point, not the final product.

Please fork, copy, modify, delete, share or do whatever you like with this.

All contributions are welcome!

## Requirements

This project requires [Node.js](http://nodejs.org) v4.x.x  to be installed on your machine. Please be aware that you may encounter problems with the installation if you are using v5.1.0 with all the latest features.

FoundationPress uses [Sass](http://Sass-lang.com/) (CSS with superpowers). In short, Sass is a CSS pre-processor that allows you to write styles more effectively and tidy.

The Sass is compiled using libsass, which requires the GCC to be installed on your machine. Windows users can install it through [MinGW](http://www.mingw.org/), and Mac users can install it through the [Xcode Command-line Tools](http://osxdaily.com/2014/02/12/install-command-line-tools-mac-os-x/).

If you have not worked with a Sass-based workflow before, I would recommend reading [FoundationPress for beginners](https://foundationpress.olefredrik.com/posts/tutorials/foundationpress-for-beginners), a short blog post that explains what you need to know.

## Quickstart

### 1. Clone the repository and install with npm
```bash
$ cd my-wordpress-folder/wp-content/themes/
$ git clone https://github.com/olefredrik/FoundationPress.git
$ cd FoundationPress
$ npm install
```

### 2. While you're working on your project, run:

```bash
$ npm run watch
```

If you want to take advantage of browser-sync (automatic browser refresh when a file is saved), simply open your Gulpfile.js and put your local dev-server address (e.g localhost) in this field ```var URL = '';``` , save the Gulpfile and run
```bash
$ npm run watch
```

### 3. For building all the assets, run:

```bash
$ npm run build
```

Build all assets minified and without sourcemaps:
```bash
$ npm run production
```

### Styles

 * `style.css`: Do not worry about this file. (For some reason) it's required by WordPress. All styling are handled in the Sass files described below

 * `assets/scss/foundation.scss`: Make imports for all your styles here
 * `assets/scss/global/*.scss`: Global settings
 * `assets/scss/components/*.scss`: Buttons etc.
 * `assets/scss/modules/*.scss`: Topbar, footer etc.
 * `assets/scss/templates/*.scss`: Page template spesific styling

Please note that you **must** run `npm run build` or `npm run watch` in your terminal for the styles to be copied and concatenated. See the [Gulpfile.js](https://github.com/olefredrik/FoundationPress/blob/master/gulpfile.js) for details

### Scripts

* `assets/javascript/custom`: This is the folder where you put all your custom scripts. Every .js file you put in this directory will be minified and concatenated one single .js file. (This is good for site speed and performance)

Please note that you must run `npm run build` or `npm run watch` in your terminal for the scripts to be copied and concatenated. See [Gulpfile.js](https://github.com/olefredrik/FoundationPress/blob/master/gulpfile.js) for details

### The main styles and scripts generated by the build

Version control on these files are turned off because they are automatically generated as part of the build process.

* `assets/stylesheets/foundation.css`: All Sass files are minified and compiled to this file
* `assets/stylesheets/foundation.css.map`: CSS source maps

* `assets/javascript/vendor`: Vendor scripts are copied from `assets/components/` to this directory. We use this path for enqueing the vendor scripts in WordPress.

### Check For WordPress Coding Standards

Foundation comes with everything you need to run tests that will check your theme for WordPress Coding Standards. To enable this feature you'll need to install PHP Codesniffer, along with the WordPress Coding Standards set of "Sniffs". You'll need to have [Composer](https://getcomposer.org/) To install both run the following:
```bash
$ composer create-project wp-coding-standards/wpcs:dev-master --no-dev
```
When prompted to remove existing VCS, answer Yes by typing `Y`.

Once you have installed the packages, you can check your entire theme by running:
```bash
$ npm run phpcs
```

If there are errors that Code Sniffer can fix automatically, run the following command to fix them:
```bash
$ npm run phpcbf
```

## Demo

* [Clean FoundationPress install](http://foundationpress.olefredrik.com/)
* [FoundationPress Kitchen Sink - see every single element in action](http://foundationpress.olefredrik.com/kitchen-sink/)

## Unit Testing With Travis-CI

FoundationPress is completely ready to be deployed to and tested by Travis-CI for WordPress Coding Standards and best practices. All you need to do to activate the test is sign up and follow the instructions to point Travis-CI towards your repo. Just don't forget to update the status badge to point to your repositories unit test.
[Travis-CI](https://travis-ci.org/)

## UI toolkits for rapid prototyping

* [Foundation UI Kit for Axure RP](https://gumroad.com/l/foundation-ui-kit-axure-rp)
* [FoundationPSD - Foundation UI Kit for Photoshop](http://foundationpress.olefredrik.com/downloads/foundation-psd-template/)

## Tutorials

* [FoundationPress for beginners](https://foundationpress.olefredrik.com/posts/tutorials/foundationpress-for-beginners/)
* [Responsive images in WordPress with Interchange](http://rachievee.com/responsive-images-in-wordpress/)
* [Build a Responsive WordPress theme](http://www.webdesignermag.co.uk/build-a-responsive-wordpress-theme/)
* [Learn to use the _settings file to change almost every aspect of a Foundation site](http://zurb.com/university/lessons/66)
* [Other lessons from Zurb University](http://zurb.com/university/past-lessons)

## Documentation

* [Zurb Foundation Docs](http://foundation.zurb.com/docs/)
* [WordPress Codex](http://codex.wordpress.org/)

## Showcase

* [Harvard Center for Green Buildings and Cities](http://www.harvardcgbc.org/)
* [INTI International University & Colleges](http://international.newinti.edu.my/)
* [Conservative Leadership Conference](http://civitasclc.com/)
* [The New Tropic](http://thenewtropic.com/)
* [Parent-Child Home Program](http://www.parent-child.org/)
* [Hip and Healthy](http://hipandhealthy.com/)
* [Threadbird blog](http://blog.threadbird.com/)
* [Public House Wines](http://publichousewine.com/)
* [Franchise Career Advisors](http://franchisecareeradvisors.com/)
* [Le saint](http://www.lesaint.ca/)
* [Help blog](http://help.com/blog/)
* [Maren Schmidt](http://marenschmidt.com/)
* [Ciancimino Gallery](http://ciancimino.com/)
* [The Rainbow Venues](http://www.therainbowvenues.co.uk/)
* [Ameronix](http://www.ameronix.com/)
* [Finnerodja](http://www.finnerodja.se/)
* [Glossop Cartons](http://www.glossopcartons.co.uk/)
* [Ready4Work](http://www.ready4work.my/)
* [Just Legal](http://www.justlegal.co.jp/en/)
* [Vintage and Stuff](http://vintageandstuff.com/)
* [Software for FM](http://softwareforfm.co.uk/)
* [WP Diamonds](http://www.wpdiamonds.com/)
* [Storm Arts](http://stormarts.fi/)
* [USS Illinois](http://ussillinois.org/)
* [OffGrid Magazine](https://offgridweb.com/)
* [Axe](http://www.axe.be/)
* [ProfitGym](http://profitgym.nl/)
* [Dr Now](http://www.drnow.com/)

>Credit goes to all the brilliant designers and developers out there. Have **you** made a site that should be on this list? [Please let me know](https://twitter.com/olefredrik)

## Contributing
#### Here are ways to get involved:

1. [Star](https://github.com/olefredrik/FoundationPress/stargazers) the project!
2. Answer questions that come through [GitHub issues](https://github.com/olefredrik/FoundationPress/issues)
3. Report a bug that you find
4. Share a theme you've built on top of FoundationPress
5. [Tweet](https://twitter.com/intent/tweet?original_referer=http%3A%2F%2Ffoundationpress.olefredrik.com%2F&text=Check%20out%20FoundationPress%2C%20the%20ultimate%20%23WordPress%20starter-theme%20built%20on%20%23Foundation%206&tw_p=tweetbutton&url=http%3A%2F%2Ffoundationpress.olefredrik.com&via=olefredrik) and [blog](http://www.justinfriebel.com/my-first-experience-with-foundationpress-a-wordpress-starter-theme-106/) your experience of FoundationPress.

#### Pull Requests

Pull requests are highly appreciated. Please follow these guidelines:

1. Solve a problem. Features are great, but even better is cleaning-up and fixing issues in the code that you discover
2. Make sure that your code is bug-free and does not introduce new bugs
3. Create a [pull request](https://help.github.com/articles/creating-a-pull-request)
4. Verify that all the Travis-CI build checks have passed
