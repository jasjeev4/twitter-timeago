# twitter-timeago: a jQuery plugin

Twitter Timeago is a jQuery plugin that makes it easy to support automatically updating timestamps in the sort of format that Twitter does (e.g. "4m" or "1d") from ISO 8601
formatted dates and times embedded in your HTML (à la microformats).

## Usage

First, load jQuery and the plugin:

```html
<script src="jquery.min.js" type="text/javascript"></script>
<script src="jquery.timeago.js" type="text/javascript"></script>
```

Now, let's attach it to your timestamps on DOM ready - put this in the head section:

```html
<script type="text/javascript">
   jQuery(document).ready(function() {
     $("abbr.timeago").timeago();
   });
</script>
```

This will turn all abbr elements with a class of timeago and an ISO 8601
timestamp in the title (conforming to the
[datetime design pattern microformat](http://microformats.org/wiki/datetime-design-pattern)):

```html
<abbr class="timeago" title="2011-12-17T09:24:17Z">September 9, 2014</abbr>
```

into something like this:

```html
<abbr class="timeago" title="December 17, 2011">1d</abbr>
```

HTML5 `<time>` elements are also supported:

```html
<time class="timeago" datetime="2011-12-17T09:24:17Z">September 9, 2014</time>
```

As time passes, the timestamps will automatically update.

**For more usage and examples**: view the index.html file

**For different language configurations**: visit the [`locales`](https://github.com/rmm5t/jquery-timeago/tree/master/locales) directory.

## Author

[Ryan McGeary](http://ryan.mcgeary.org) ([@rmm5t](http://twitter.com/rmm5t))

## Other

[MIT License](http://www.opensource.org/licenses/mit-license.php)

Copyright (c) 2008-2013, Ryan McGeary (ryan -[at]- mcgeary [*dot*] org)