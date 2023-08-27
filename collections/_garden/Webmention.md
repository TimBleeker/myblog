---
share: true
layout: garden_entry
type: _garden
---
creation: 20230227120923
tags: [[IndieWeb]], [[Web dev]]

In simple terms, the webmention is a nerdy way of speaking to other people's personal websites. Rather than writing a comment on a page, liking it, or sending the maker an email about it, we use the webmention to publish a response on our own website, and then send it in a special way.

"Special way" is a euphemism for how difficult it can be to set up webmentions.

My strategy currently consists of automatically receiving and displaying incoming webmentions. Any outgoing webmentions, sadly, are sent manually. I'm hoping to change that in the future.

### Incoming webmentions
- ~~When someone sends a webmention to one of my paged, either manually or automatically, Netlify will see it, because it checks for new webmentions every time I deploy my website using the [Webmentions build plugin](https://www.netlify.com/integrations/community-built/webmentions-build-plugin/) .~~
- ~~Because it's fetched during deployment, the webmention is automatically displayed on my website, because I use [fluffy](http://beesbuzz.biz/)'s [webmention.js](https://github.com/PlaidWeb/webmention.js).~~
- When looking up how my webmentions work for [Elliott](https://elliott.computer/), I incorrectly thought Netlify does anything to receive webmentions, but that's incorrect.
- [Webmention.io](https://webmention.io/) collects incoming webmentions for me.
- I display them on my website using [fluffy](http://beesbuzz.biz/)'s [webmention.js](https://github.com/PlaidWeb/webmention.js).

### Outcoming webmentions
Whenever I want to send a webmention to someone, perhaps because I'm replying to their content specifically (rather than mentioning their website in passing), I'll send it via [Telegraph](https://telegraph.p3k.io/).