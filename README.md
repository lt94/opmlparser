# OPML Parser

[![Build Status](https://travis-ci.org/witochandra/webfeed.svg?branch=master)](https://travis-ci.org/witochandra/webfeed)
[![Pub](https://img.shields.io/pub/v/webfeed.svg)](https://pub.dartlang.org/packages/webfeed)

A dart package for parsing OPML.

### Installing

Add this line into your `pubspec.yaml`
```
opmlparser: ^0.0.1
```

Import the package into your dart code using:
```
import 'package:opmlparser/opmlparser.dart';
```

### Example

To parse string into `OPML` object use:
```
Opml opml = Opml.parse(xmlString);
```

### Preview

**RSS**
```
feed.title
feed.description
feed.link
feed.author
feed.items
feed.image
feed.cloud
feed.categories
feed.skipDays
feed.skipHours
feed.lastBuildDate
feed.language
feed.generator
feed.copyright
feed.docs
feed.managingEditor
feed.rating
feed.webMaster
feed.ttl
feed.dc

RssItem item = feed.items.first;
item.title
item.description
item.link
item.categories
item.guid
item.pubDate
item.author
item.comments
item.source
item.media
item.enclosure
item.dc
```

**Atom**
```
feed.id
feed.title
feed.updated
feed.items
feed.links
feed.authors
feed.contributors
feed.categories
feed.generator
feed.icon
feed.logo
feed.rights
feed.subtitle

AtomItem item = feed.items.first;
item.id
item.title
item.updated
item.authors
item.links
item.categories
item.contributors
item.source
item.published
item.content
item.summary
item.rights
item.media
```

## License

WebFeed is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details