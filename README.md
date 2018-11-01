# Gitbook custom theme for andrew
This is a plugin for Gitbook, version 3.0.0 or higher

It adds a new block with logo. The andrew theme extends HTML templates, CSS styles and JS scripts of a base GitBook theme [gitbook-plugin-theme-default](https://www.npmjs.com/package/gitbook-plugin-theme-default).

The plugin can be used as a blank theme template for GitBook.

Usage
Add the theme to your book's configuration book.json:

``` 
{
    "plugins": [
        "theme-andrew@https://github.com/andrewzhyl/gitbook-plugin-theme-andrew.git"
    ],
    "pluginsConfig": {
        "theme-andrew": {
            "title": "Git Info book title",
            "logo": "/assets/300-dpi-high-resolution-logo.png",
            "favicon": "/assets/home.png",
            "footer": {
                "copyright-text": "©2017 Resereved for world",
                "links": [{
                    "title": "Home",
                    "link": "/home"
                }, {
                    "title": "About",
                    "link": "/about"
                }]
            },
            "header": {
                "links": [{
                    "title": "Home",
                    "link": "/home"
                }, {
                    "title": "About",
                    "link": "/about"
                }]
            }
        }
    }
},
```

Install by running the following command within your book's root folder:

``` bash
gitbook install
```