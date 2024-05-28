PicoFeed
========

Fork Notes
----------

Fork of : https://github.com/aaronpk/picofeed with ....

 * 2024/05/28 - add PHP8.2 support (remove PHP deprecation warnings etc), tentatively tag as v1.0.0

Use :

add e.g.
```
 ...
  "repositories" : [
        {
            "type": "vcs",
            "url" : "git@github.com:DavidGoodwin/picofeed.git"
        }
   ],
   ...
```

to your composer.json and then e.g. ` "p3k/picofeed": "^1.0" `


Original Readme
---------------

PicoFeed was originally developed for [Miniflux](http://miniflux.net), a minimalist and open source news reader.

[![Build Status](https://travis-ci.org/aaronpk/picoFeed.svg?branch=master)](https://travis-ci.org/aaronpk/picofeed)

This fork of PicoFeed was created after the original author dropped support. It is published on Packagist as `p3k/picofeed`.

```
composer require p3k/picofeed
```

Features
--------

- Simple and fast
- Feed parser for Atom 1.0 and RSS 0.91, 0.92, 1.0 and 2.0
- Feed writer for Atom 1.0 and RSS 2.0
- Favicon fetcher
- Import/Export OPML subscriptions
- Content filter: HTML cleanup, remove pixel trackers and Ads
- Multiple HTTP client adapters: cURL or Stream Context
- Proxy support
- Content grabber: download from the original website the full content
- Enclosure detection
- RTL languages support
- License: MIT

Requirements
------------

- PHP >= 5.3
- libxml >= 2.7
- XML PHP extensions: DOM and SimpleXML
- cURL or Stream Context (`allow_url_fopen=On`)
- iconv extension

Authors
-------

- Original author: Frédéric Guillot
- Major Contributors:
    - [Bernhard Posselt](https://github.com/Raydiation)
    - [David Pennington](https://github.com/Xeoncross)
    - [Mathias Kresin](https://github.com/mkresin)

Real world usage
----------------

- [Miniflux](http://miniflux.net)
- [Owncloud News](https://github.com/owncloud/news)
- [XRay](https://github.com/aaronpk/xray)
- [Aperture](https://aperture.p3k.io)

Documentation
-------------

- [Installation](docs/installation.markdown)
- [Running unit tests](docs/tests.markdown)
- [Feed parsing](docs/feed-parsing.markdown)
- [Feed creation](docs/feed-creation.markdown)
- [Favicon fetcher](docs/favicon.markdown)
- [OPML](docs/opml.markdown)
- [Image proxy](docs/image-proxy.markdown) (avoid SSL mixed content warnings)
- [Web scraping](docs/grabber.markdown)
- [Exceptions](docs/exceptions.markdown)
- [Debugging](docs/debugging.markdown)
- [Configuration](docs/config.markdown)
