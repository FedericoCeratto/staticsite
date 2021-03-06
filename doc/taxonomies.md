## Taxonomies

Any number of taxonomies, each described by a `<name>.taxonomy` file where it
should appear in the site.

See `example/content/tags.taxonomy` for details.

```toml
+++
# In staticsite, a taxonomy is a group of attributes like categories or tags.
#
# Like in Hugo, you can have as many taxonomies as you want. See
# https://gohugo.io/taxonomies/overview/ for a general introduction to
# taxonomies.
#
# This file describes the taxonomy for "tags". The name of the taxonomy is
# taken from the file name.
#
# The format of the file is the same that is used for the front matter of
# posts, again same as in Hugo: https://gohugo.io/content/front-matter/

# Singular name for an element of the taxonomy
item_name = "tag"

# Output directory for the tag index, tag pages and Atom/RSS2 feeds.
# The path is relative to this file.
output_dir = "tags/"

# Template for rendering the taxonomy index. Here, it's the page that shows the
# list of tags
template_tags = "tags.html"

# Template for rendering the page for one tag. Here, it's the page that shows
# the latest pages tagged with the tag
template_tag = "tag.html"

# Template for rendering the archive page for one tag. Here, it's the page that
# links to all the pages tagged with the tag
template_archive = "tag-archive.html"

# Templates for rendering the Atom and RSS2 feeds for each tag
template_atom = "tag.atom"
template_rss = "tag.rss"

# When pages are added with these items of this taxonomy, also add them to a
series with the same name as the tag
serires = ["links", "songs"]
+++
```

[Back to README](../README.md)
