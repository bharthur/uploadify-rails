# uploadify-rails

This gem provides the Uploadify jQuery plugin for your Rails 3.1+ app.

For more information about Uploadify, visit http://www.uploadify.com/

## Requirements

* jQuery (e.g. from the [jquery-rails](https://github.com/rails/jquery-rails) plugin)

## Installation

Add the gem to your Gemfile:

    gem 'uploadify-rails', :git => 'https://github.com/lucaspiller/uploadify-rails.git'

Then run `bundle install`.

### Rails 3.1 or greater (with asset pipeline enabled)

Add this to `app/assets/javascripts/application.js`:

    //= require uploadify

For the default styles, add this to `app/assets/stylesheets/application.css`:

    *= require uploadify

## Usage

See the [Uploadify docs](http://www.uploadify.com/documentation/) for full customisation options. A simple example if as follows, where `#user_picture_upload` is a file input field:

    $(function() {
      $("#user_picture_upload").uploadify({
        height        : 30,
        uploader      : '/user/pictures',
        width         : 120
      });
    });

TODO: Server side implementation docs.
