Okay, so this one is a slightly complicated topic with a lot of details but a lot of these things you might never use, there will be libaries silently handling all the complexity for you. If you are curious though, follow along!

First let's start with what routing is. Routing simply meant - given a URL, the server will return a particular resource and for different URLs, the server will return different resources. For now, let's not focus on what a 'resource' might be. 

Until a couple of years ago, servers used to return HTML pages in response to different routes. Take GitHub for instance. For different pages on the site, you will see different markup being returned. 

As the client libraries got better and the JavaScript layers got thicker, someone asked - 

> Hey, if I am showing the same navbar, the same footer and the same JS file for each route, why do I need to send it across the wire each time? Can't the client only ask for what it needs?

The question had merit and so began client-side routing. Simply put, clients trade with servers on data while it holds the markup required to render different routes. This way, whenever a route changes, only the differences are rerendered, the rest of the page stays as is. 

The implementation of client-side routing is not straight-forward and is wrought with browser quirks. Here are some articles to check out if you are curious how it works - 

1. https://stackoverflow.com/a/37062379
2. http://krasimirtsonev.com/blog/article/deep-dive-into-client-side-routing-navigo-pushstate-hash



**Note** - A lot of learning happens on our community Slack channel. If you aren't there already, [click here](https://join.slack.com/t/proso-io/shared_invite/enQtNjAyNjA3MzY4MDY3LWI4MDFmMzQwNjkyNjdhMGQyOTYzNjM4YTllOTkxYjI5YzY4NmFjMDhiMTM2ZWNlMGI1NzEwMzAxOTc0YTgwYzA) to join the community.
