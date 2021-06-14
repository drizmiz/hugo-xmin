# HUGO XMIN+

This repository is basically `yihui/hugo-xmin` with some additional simple features and widgets. Changes include:

- Change `permalinks` from "/:year/:month/:day/"-like to "/:year/"-like

- Remove the "Subscribe" term

- +GithubEdit

- Change the footer of the example site from copyright to CC-BY-SA 3.0 flavored copyleft

- Change the sources of some js files

- +some fonts and css

- Embed Disqus (powered by DisqusJS)

- Show categories and tags for each post

This repository is re-licensed under the terms of **MPL v2.0**. The original MIT license is preserved and renamed to `MITLicense_Xie.md`.

The original documentation is kept as-is below.

## _Keep it simple, but not simpler_

**XMin** is a Hugo theme written by [Yihui Xie](https://yihui.org) in about four hours: half an hour was spent on the Hugo templates, and 3.5 hours were spent on styling. The main motivation for writing this theme was to provide a really minimal example to beginners of Hugo templates. This XMin theme contains about 130 lines of code in total, including the code in HTML templates and CSS (also counting empty lines).


```bash
find . -not -path '*/exampleSite/*' \( -name '*.html' -o -name '*.css' \) | xargs wc -l
```

```
       5 ./layouts/404.html
      12 ./layouts/_default/single.html
      20 ./layouts/_default/list.html
      13 ./layouts/_default/terms.html
       0 ./layouts/partials/foot_custom.html
       0 ./layouts/partials/head_custom.html
       9 ./layouts/partials/footer.html
      20 ./layouts/partials/header.html
      51 ./static/css/style.css
       7 ./static/css/fonts.css
     137 total
```

I can certainly further reduce the code, for example, by eliminating the CSS, but I believe a tiny bit of CSS can greatly improve readability. You cannot really find many CSS frameworks that only contain 50 lines of code.

[![Screenshot](https://github.com/yihui/hugo-xmin/raw/master/images/screenshot.png)](https://xmin.yihui.org)
