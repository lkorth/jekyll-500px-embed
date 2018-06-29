jekyll-500px-embed
==================

# End of Life

On June 15th, 2018 500px [shut off their API](https://support.500px.com/hc/en-us/articles/360002435653-API-). jekyll-500px-embed used the 500px API to retrieve information about a photo in order to render the embedded html and no longer functions without the API.

## Installation

1. Copy `500px_tag.rb` into your site's `plugins` directory.
2. Create a file containing a 500px API consumer key in the root directory of your site.
A consumer key can be obtained by [creating an app with 500px](https://500px.com/settings/applications).
3. Add the file containing your consumer key to your `.gitignore`.
4. Add the following to your `_config.yml`

  ```yaml
  500px_consumer_key_file: 500px-consumer-key
  ```

  where `500px-consumer-key` is the name of the file created in #2.

5. Add the following javascript to any page you wish to use the plugin on, or use the included [copy](500px-embed.js).

  ```html
  <script src="//500px.com/embed.js" type="text/javascript"></script>
  ```

## Usage

Supply the photo id you wish to embed to the 500px tag. The photo id can be found in the photo's url on [http://500px.com](http://500px.com).

```markdown
{% 500px 89255597 %}
```

## Example

[https://lukekorth.com/blog/500px-embedding-for-jekyll/](https://lukekorth.com/blog/500px-embedding-for-jekyll/)
