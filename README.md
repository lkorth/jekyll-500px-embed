jekyll-500px-embed
==================

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

```markdown
{% 500px 89255597 %}
```

## Example

[https://lukekorth.com/blog/500px-embedding-for-jekyll/](https://lukekorth.com/blog/500px-embedding-for-jekyll/)
