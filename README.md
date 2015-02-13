<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc/generate-toc again -->
**Table of Contents**

- [Andrei's side project ideas](#andreis-side-project-ideas)
    - [Web services](#web-services)
        - [Sidelog](#sidelog)
        - [Death.app](#deathapp)
        - [Agreed](#agreed)
        - [EtiCo](#etico)
        - [Badger](#badger)
        - [Mink](#mink)
        - [Social collage](#social-collage)
        - [Mockery](#mockery)
        - [Algo](#algo)
        - [Calendar match](#calendar-match)
        - [Imgur for CSV](#imgur-for-csv)
        - [Cloud extender](#cloud-extender)
        - [Github comments](#github-comments)
        - [Imgur vigilante](#imgur-vigilante)
    - [OSS](#oss)
        - [OSXinit](#osxinit)
        - [new](#new)
        - [Cloud ORM](#cloud-orm)
        - [Darling](#darling)
        - [markdoc](#markdoc)
    - [Fun](#fun)
        - [Hahazon](#hahazon)
        - [Programming languages map](#programming-languages-map)
        - [WAOTD](#waotd)
        - [Learned](#learned)
        - [Postgrid](#postgrid)

<!-- markdown-toc end -->

# Andrei's side project ideas

Some ideas I had over the past couple of years. I'm making it public based on the principle that [ideas are cheap](https://www.google.com/search?q=ideas+are+cheap).

Yes, the names are silly, they're just codenames to make referencing easier.

## Web services

### Sidelog

*The meta side-project idea*

A service for storing side-project ideas.

Features:

* Zero knowledge is important for the users' peace of mind (also, why not?).
* Sharing ideas with friends, or with the `sidelog` commmunity. It's easier to start working on something together.
* Informal equity-splitting agreement. (something to point to when someone offers to buy your silly side project for 1 cool million)

### Death.app

People die, data and online profiles don't. `death-app` is a way of letting your loved ones get your online data and delete/edit your public profiles after you die.

A *very* similar idea came up on HN some time ago and people dismissed it as mostly a social/legal challenge, *but* their implementation was pretty crappy.

### Agreed

A web service for informal agreements. Not legally enforceable, but any party can make an agreement public.

Features:

* Email-driven; there's no easy way of establishing "real" identity on the Internet, so an agreement must happen between email addresses, not *people*. This also means that confirmation happens via email.
* Public *and* private/unlisted agreements. As I said, any party can make an agreement public if unsatisfied.

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

* Mobile apps that can scan barcodes; quite often when shopping you'll have several very similar options, this might be a good way to differentiate between them.


### Badger

Pinboard.in on steroids. A read-it-later-probably-never service for interesting content (TED talks, tech documents, etc). Adding metadata (tags) to the bookmarks can develop in interesting ways. Pinboard.in does the first part right, but they don't leverage the data. Having a meaningful categorization layer over what people find intersting is bound to have some interesting use cases. Two obvious ones: "interesting stuff of the day" and "interesting stuff in your field".

Problems:

* Not clear how it differentiates from existing services
* Dead links (webarchive or pinboard.in archiving feature)

Ideas:

* Pinboard integration: Can it be developed on top of pinboard.in? Their db isn't bad, and the cost of building a ecosystem in this area is very high.
* Intelligent *complex resource* detection: A bookmark can contain more than one link (think Youtube playlist, MOOC course, etc.). Therefore, a way of mapping a bookmark to a set of links or ID might be useful.

*(Both badgers and minks are cute, furry animals, and badgers hoard stuff (URLs, most likely) in their underground burrows. I did warn you the names were stupid.)*

### Mink

![mink pic](http://i.imgur.com/mFHxoGa.jpg)

**M**ulti-l**ink** URL shortener. Pretty straight-forward, instead of `short.url/:id` -> `expanded.url/path/to/content`, a short URL expands to multiple links.

The default can be to show all the URLs on a page, open all or some of them in new tabs. Appending `/open` to the URL could skip showing the preview page and just open `N` tabs.

### Social collage

Some events throw around hashtags for posting to social media. Hackathons and conferences are a good example of this. That means that it's pretty straightforward to extract all media (i.e. photos and videos?) from Twitter/Instagram/Facebook for specific **hashtags**, **dates**, and **places**. Thus, the idea of quickly generating a media collage from an event by specifying a hashtag and optionally other parameters.

![balsamiq mockup](http://i.imgur.com/XHbHG25.png)

### Mockery

A website for collaborative mock interviews for people preparing for technical interviews.

Features:

* Ratings are essential.
* Holding and getting interviews must be balanced.
* Being interviewed by higher levels costs money (the interviewer should get 80%+).
* Fast track to a high level if you work for a top company. Incentive: earn money while sharpening your interview skills; go pro bono if you want to give back to society.

PS: If you build this without me I'll be very sad.

### Algo

Goodreads for algorithms, sort of. A database of algorithms useful for exploring new algorihtms in a structured fashion. Users can map the algorithms they already know, and either add items to their "To Learn" list, or choose a category/subtree to learn more about (e.g. machine learning, sorting algorithms, game algorithms, etc).

Similar:

* [Rosetta Code](http://rosettacode.org/wiki/Rosetta_Code)
* [Algorithmia](https://algorithmia.com/)

### Calendar match

Find when everyone is available for a meeting. Google Calendar seems to have a [builtin feature to do that](https://support.google.com/calendar/answer/178219), however nothing like this that's simple and cross-platform seems to exist. Something that works with gcal/outlook would be a great start. Outlook provides add-ins, and for Google Calendar a browser plugin might be appropriate.

### Imgur for CSV

The next Instagram/Whats App hybrid that will change the world and revolutionize how you buy hispter clothes online.

A simple service to upload, host, and display CSVs or other tabular file formats. Might feature interesting public data sets on the front page. Example, a [researcher just published 10 million username/password pairs](https://xato.net/passwords/ten-million-passwords/).

Not necessarily for large public data sets (you can find more [here](https://www.quora.com/Where-can-I-find-large-datasets-open-to-the-public), check it out). Uploading bigger files could be a premium feature.

(This could as well be a Github Gist visualization feature.)

### Cloud extender

A tool that creates a virtual filesystem from multiple cloud storage accounts. Just between Google Drive, Streamnation, and OneDrive you can get 50GB of free storage.

Features:

* faster speeds as multiple back ends are used
* redundancy is an option, files can have replicas
* bonus, a chance to get banned from these services for life

### Github comments

Sometimes Github repos feel like they could use a simple imgur-like commenting system. Gitter does a good job of providing a chat interface to a repository, although the fact that it's not widely used speaks for how useful that feature is (i.e. popular projects use IRC, for non-popular ones an issue usually is enough communication). `github-comments` would be a simple service that just adds a commenting layer on top of repositories.

How to access comment page:

1. `github.com/repo` -> `github-comments.com/repo`
2. Install a browser plugin. Notification count shows at a glance how many comments a page has.

### Imgur vigilante

`imgur-vigilante` is a browser extension to mass-[up|down]vote on Imgur

## OSS

### OSXinit

Mac configuration backup. The aim is to make the transition to a new computer as quick as possible.

Look up:

* https://github.com/lra/mackup
* https://dotfiles.github.io/

### new

Plugin-based utility to create *new* stuff.

Examples:

```lang=shell
new tw Hello, World from new-twitter                 # posts to Twitter
new todo Remember the milk at 8pm                    # integrates with some task managers
new trello board --template kanban user/board-name   # new Trello board, duh
new install twitter                                  # builtin plugin to install other plugins
new update/upgrade/up (update+upgrade)               # builtin plugins for upgrading new or the plugins
new config export/import/clone/sync                  # builtin commands for new and plugins config
```

Would this be useful? No idea. But it'd be fun to write.

### Cloud ORM

Misnomer, a unified API for cloud storage services like Google Drive and Dropbox.

Similar to what segment.io does for tracking providers.

Update: Annoyingly, this exists: https://news.ycombinator.com/item?id=8442004

### Darling

A Chromium fork that handles better languages (DARt, Less, etc.) without compiling them to html/css/js.

Alternatively, a browser built from the ground up to support something cool like [elm](http://elm-lang.org/).

### markdoc


I've never managed to find a simple, good, self-hosted, Markdown-based wiki. [Markdoc](https://github.com/zacharyvoase/markdoc) is the closest to what I have in mind, and it's abandoned/the author seems happy to hand the project to another maintainer.

Go might be a good language for this application, there's already a good, fast static website generator written in it: http://gohugo.io/


## Fun

### Hahazon

A website to collect funny Amazon reviews. Copyright issues are murky - ethically, the reviewers are entitled to earnings, legally probably Amazon would have a word or two to say. A book can *easily* be released, since items are a good fit for that (basically 1 or more photos + some text).


### Programming languages map

Related: https://news.ycombinator.com/item?id=7100341

I can't exactly what I had in mind with this, but a graph based on certain lang characteristics (compiled/interpreted, age, paradigms, platforms, proximity to hardware, etc.) would be useful I guess.

### WAOTD

Wikipedia Article Of The Day. The simplest application, can be a good programming exercise when learning a new language.

### Learned

A way of keeping track of your knowledge. Pretty hazy how this could be implemented. A simple solution can be via `badger`, i.e. just save the links or description of the material studied (example: CLRS, Crash Course videos on Youtube, a Udacity course, etc.).

### Postgrid

A post-apocalyptic way of connecting people. We tend to take for granted rather fragile networks that can be taken apart by war or cosmic events. It shouldn't rely on satellites or any kind of grid, and use common electronic items i.e. laptops, smartphones, wireless routers. Also, it should be easy to use by everyone and not require installation.

Ideas:

* USB stick communication. Offline social network based on a public broadcast, append-only model. Whenever 2 devices interact they sync themselves by downloading the other's changes to the network state. Inspired by: [deaddrops](https://deaddrops.com/)
* WAN-type ad-hoc network using laptops and wireless routers.
* Smartphone wiper. Most (?) smartphones are useless without a network. This should be something that can break any device and install a useful yet low-tech OS. One handy feature is related to the offline social network mentioned - the device could automatically sync with other devices that get in its radius.

This could work because only 2 people need to have to software: the ones setting up the USB sticks, and the ones that can wipe the mobile devices.
