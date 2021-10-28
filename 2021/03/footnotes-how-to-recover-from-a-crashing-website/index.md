# footnotes: How to recover from a crashing website


Dear footnotes community,

We recently accidentally shipped a version of our plugin that might break your website.
Apologising [here](https://cheret.org/2021/03/footnotes-2.5.10-reverts-2.5.9d1-and-apologies/).

## How to recover from a crashing website?

Fellow footnotes user @pppierreee pointed out that it would be helpful to give you guidance how to recover:

– Download [footnotes 2.5.8](https://downloads.wordpress.org/plugin/footnotes.2.5.8.zip)
– Unzip
– Delete the wp-content/plugins/footnotes/ folder on your webserver
– Upload the contents of the unzip (the footnotes folder) to wp-content/plugins/

## What happens to your footnotes?

Your footnotes are untouched by this, as they live in your posts and pages and are not stored in the plugin.

