{
    "title":"GO-Fastly updates",
    "link":"https://github.com/sethvargo/go-fastly/pulls?q=is%3Apr+author%3Ajare19+is%3Aclosed",
    "image":"/img/fastly.png",
    "description":"Go Fastly is a Golang API client for interacting with most facets of the Fastly API.",
    "tags":["Go","GoLang","Fastly","WAF","Cloud Security","CDN"],
    "weight":"10",
    "sitemap": {"priority": "0.8"},
    "featured": true
}

[![Go Documentation](http://img.shields.io/badge/go-documentation-blue.svg?style=flat-square)][godocs]

[godocs]: http://godoc.org/github.com/sethvargo/go-fastly

Go Fastly is a Golang API client for interacting with most facets of the
[Fastly API](https://docs.fastly.com/api).

There was an API endpoint missing from the go-fastly API client, Event Logs. I added the event logs endpoint to the package as well as all the tests. I also noticed that the returned objects for the dictionary objects and items were not up to date so I updated those as well.