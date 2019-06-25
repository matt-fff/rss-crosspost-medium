# medium-crosspost
[![DUB](https://img.shields.io/dub/l/vibe-d.svg)]()
[![Dependabot Status](https://api.dependabot.com/badges/status?host=github&repo=typenil/rss-crosspost-medium)](https://dependabot.com)
[![Build Status](https://travis-ci.org/typenil/rss-crosspost-medium.svg?branch=master)](https://travis-ci.org/typenil/rss-crosspost-medium)
[![Test Coverage](https://api.codeclimate.com/v1/badges/ab4e0c7281d017107371/test_coverage)](https://codeclimate.com/github/typenil/rss-crosspost-medium/test_coverage)
[![Maintainability](https://api.codeclimate.com/v1/badges/ab4e0c7281d017107371/maintainability)](https://codeclimate.com/github/typenil/rss-crosspost-medium/maintainability)


A Python script to crosspost articles to Medium.

Accompanies [this blog post](https://typenil.com/automatic-rss-medium-cross-posting/), which goes into depth on crossposting to [Medium](https://medium.com/) from an RSS feed via [Zapier](https://zapier.com/).

## Installation:
 
`pip install medium-crosspost-rss`


## Basic Usage:

```
from medium_crosspost import MediumCrosspost

input_data = {
    "title": "Fantastic Article Name!",
    "canonicalUrl": "https://www.example.com/fantastic-article-name",
    "integrationToken": "super-secret-medium-integration-token",
    "content": "<html><head></head><body>Content is all about actual HTML-encoded article content.</body></html>",
    "tags": "can,be,a,list,or,comma,separated,string",
}

crosspost = MediumCrosspost(input_data)
result = crosspost.post()
```
