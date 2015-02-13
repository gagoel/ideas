This is a list of project ideas that I had over time. I'm making it public based on the principle that [ideas are cheap](https://www.google.com/search?q=ideas+are+cheap).

Yes, the names are silly, they're just codenames to make referencing easier.

## Products

### Sidelog

*The meta side-project idea*

A service for storing side-project ideas. Zero knowledge is important. Features for sharing ideas with friends, or with the `sidelog` commmunity, are important – it's easier to start working on something together. A feature for informal equity-splitting agreement might be useful. (you don't want to accidentally come up with the next Instagram and not have a way of splitting the cash, right?)

### Death.app

People die, online profiles and data don't. A way of letting your loved ones get your online data and cancel your public profiles after you die.

A *very* similar idea came up on HN some time ago and people dismissed it as mostly a social/legal challenge, *but* their implementation was pretty crappy.

### Agreed

A web service for informal agreements. Not legally enforceable, but relying on the public aspect of it.

Features:

* email-driven; there's no easy way of establishing "real" identity on the Internet, so an agreement must happen between x@domain.com, y@other.domain.com, etc.
* public *and* private/unlisted; public agreements are just that, private ones can be made public by any of the participants in case of unsatisfactory results

Use cases:

* lending money to a friend
* signing an NDA before an interview (like those are ever enforced)
* signing a contract when buying a house (joke!)

### EtiCo

How ethical is a company? A crowd-sourced way of establishing this. It can work via votes, reviews, posting news articles, etc. but ideally each company would get a big `x out of 100` score.


Gotchas:

* Big Corp. will try to sue the heck out of this if they get bad reviews; a decentralised approach might fix this but make monetization impossible
* Even if you somehow prevent spamming, Samsu... uh I mean Big Corp. will pay hundreds of honest, independent reviewers to fix their ratings

Fun ideas:

* Mobile apps that can scan barcodes; some times when shopping you get several otherwise identical products, this might be a good way to differentiate between them.


### Badger

Pinboard.in on steroids. A read-it-later-more-probably-never service for interesting content (TED talks, tech documents, etc). Adding metadata (tags) to the bookmarks can develop in interesting ways. Pinboard.in does the first part right, but they don't leverage the data. Having a meaningful categorization layer over what people find intersting is bound to have some interesting use cases. Two obvious ones: "interesting stuff of the day" and "interesting stuff in your field".

Problems:

* Not clear how it differentiates from existing services
* Dead links (webarchive or pinboard.in archiving feature)

Ideas:

* Pinboard integration: Can it be developed on top of pinboard.in? Their db isn't bad, and the cost of building a ecosystem in this area is very high.
* Intelligent *complex link* detection: A bookmark can be more complex than a link (Youtube playlist, Courser course, etc.). Therefore, a way of mapping a bookmark to a set of links might be useful.

PS: It's called Badger because it relates to the next idea, and they're both furry and cute.

### Mink

![mink pic](http://i.imgur.com/mFHxoGa.jpg)

**M**ulti-l**ink** URL shortener. Pretty straight-forward, instead of `short.url/:id` -> `expanded.url/path/to/content`, a short URL expands to multiple links.

The default can be to show all the URLs on a page, open all or some of them in new tabs. Appending `/open` to the URL could skip showing the preview page and just open `N` tabs.

### Social collage

Some events throw around hashtags for posting to social media. Hackathons and conferences are a good example of this. That means that it's pretty straightforward to extract all media (i.e. photos and videos?) from Twitter/Instagram/Facebook for specific **hashtags**, **dates**, and **places**. Thus, the idea of quickly generating a media collage from an event by specifying a hashtag and optionally other parameters.

![balsamiq mockup](http://i.imgur.com/XHbHG25.png)

