## Installation

First, add the module import to your site or theme component's configuration's module section:

```toml
[module]
[[imports]]
path = "github.com/bep/hugo-jslibs/instantpage"
```

Then add the script source before the end body tag:


```html
<body>
...
{{ partial "jslibs/instantpage/script-src.html" "-" }}
</body>
```

See the [instant.page](https://instant.page/) documentation for configuration.