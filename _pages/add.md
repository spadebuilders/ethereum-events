---
layout: single
title: Add Your Event
permalink: /add/
sidebar:
  - image: assets/fellowship-logomark.png
  - image_alt: "Fellowship Logo"
  - text: "<a href='https://github.com/ethereum-magicians/scrolls'>Github Repo</a>"
  - text: "<a href='https://github.com/ethereum-magicians/scrolls/issues'>Github Issues</a>"
  - title: "Theme"
  - text: "<a href='https://mmistakes.github.io/minimal-mistakes/docs/layouts/#table-of-contents'>Table of Contents</a>"
  - text: "<a href='https://mmistakes.github.io/minimal-mistakes/docs/layouts/#custom-sidebar-content'>Custom Sidebar Content</a>"
---

This is not meant to be an exhaustive list of all Ethereum events everywhere. The event should be a community event, which generally means low- or no-cost to attendees, and inclusive.


## How to Add Your Event

To add your event, you can either:

1. Make a pull request to the Scrolls repo: [github.com/ethereum-magicians/scrolls](https://github.com/ethereum-magicians/scrolls), or
1. [File an issue](https://github.com/ethereum-magicians/scrolls/issues) with details about your event, and a volunteer will create the Jekyll post for you

The basic info to include is:
- name of your event (this is ```title```)
- brief description (```excerpt```)
- start date
- end date
- location

The format looks like:
```
title: My Awesome Event
excerpt: "My awesome event will include so many EIPs and lots of open source pull requests."
event:
  start_date: 2018-07-14T16:20:02-05:00
  end_date: 2018-07-15T16:20:02-05:00
  location: Berlin, Germany
```

If you include a ```link``` entry, then the post will link to your event website rather than focusing on a local event page.

Add links to your registration page, forum threads, or other information in the body of your event post -- or highlight it in your excerpt.

## Customizing your event page

The Jekyll theme we use is Minimal Mistakes. The [helpers documentation](https://mmistakes.github.io/minimal-mistakes/docs/helpers/) has lots of examples of what you can use in an event post.

The [Council of Berlin event page](/event/2018-council-of-berlin/) is an example of a highly customized page that can be used as a full landing page for your event.

### Table of Contents

The table of contents feature will give you a right hand table of contents based on the headers you use in the body of your post.

```
toc: true
toc_sticky: true
```

### Sidebar

You can include sidebar links, which appear at the left.

```
sidebar:
  - title: "Title"
    image: http://placehold.it/350x250
    image_alt: "image"
    text: "Some text here."
  - title: "Another Title"
    text: "More text here."
```
