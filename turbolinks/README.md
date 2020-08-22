## Description

This module wraps [Turbolinks](https://github.com/turbolinks).

Also, if [Alpine](../alpinejs/alpine) is present, it adds a set of event listeners that
prepares/cleans the AlpineJS state. Most importantly, it pauses Alpine's mutation observer so Turbolinks can do its work without interuption.

## Installation

First, add the module import to your site or theme component's configuration's module section:

```toml
[module]
[[imports]]
path = "github.com/bep/hugo-jslibs/turbolinks"
```

Then add the script source in the head section of your template (typically in the `baseof.html`):


```html
<head>
{{ partialCached "jslibs/turbolinks/script-src.html" "-" }}
</head>
```

