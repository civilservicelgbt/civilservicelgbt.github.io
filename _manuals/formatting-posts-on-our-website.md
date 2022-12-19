---
# Adding or removing a '#' in front of a line will toggle that information off and on from being processed. 

layout: manual
title: "Formatting posts on our website"
excerpt: "Learn how to format posts for the website using Markdown."
category: website
permalink: /manual/format-a-post
breadcrumbs-override: true
breadcrumbs:
- title: "Tools"
  url: /tools
- title: "Manuals"
  url: /manuals
---

Posts on this website are generated from plain text files. Each text file has either the extension:

- `.md` – which means it is formatted using Markdown syntax
- `.html` – which means it is a more advanced HTML web page

When the site builds, it takes the plain text files and generates a web page for each file on the site. This guide will tell you how to format text using Markdown syntax. 

You should use Markdown syntax when you add files using one of [our tools](/tools).

## Regular paragraph text

Regular paragraph text is any text that is on a standalone line. No additional markup is required. Always leave an empty line between paragraphs.

This paragraph is an example of how regular paragraph text is displayed.

To write this in Markdown, you would write:

```
Regular paragraph text is any text that is on a standalone line. No additional markup is required. 

This paragraph is an example of how regular paragraph text is displayed.
```

## Formatting regular paragraph text

You can make text _italic_ and **bold** by using special characters around words, phrases or sentences. 

### Bold text

To make text bold, you surround the text with `**`. Do not leave a space between the two asterisks and the words you want to display in bold. For example:

```
**This text would be bold.**
```

### Italic text

To make text bold, you surround the text with `*` or `_`. Do not leave a space between the two asterisks and the words you want to display in bold. For example:

```
*This text would be italic.*

_This text would be italic too._
```

## Headings

You can generate a heading by using a `#`, followed by a space at the start of a new line, followed by the heading you want to create. Use more `#` symbols to create sub-headings. You **must** leave a blank line before and after each heading or it will not format correctly.

For example:

```
# This is a level 1 heading

## This is a level 2 heading

### This is a level 3 heading

### This is a level 4 heading
```

Headings are **not** decorative – they have meaning. Only use a heading when you want to create a new section of content; don't use it to make things arbitrarily stand out.

Use headings in order from largest to smallest. In most cases, **do not** use the level 1 heading; the level 1 heading is usually the page title.

## Add a hyperlink

Hyperlinks (or links, for short) are ways to direct users to other pages or resources. To create a link, surround the text you want to be the link with `[ ]`, followed by `( )` containing the URL to the resource you are linking to. For example:

```
You can add a link to the [home page](https://www.civilservice.lgbt/) like this
```

You can also link to email addresses by surrounding them with `< >`. For example:

```
You can contact us via email at <info@civilservice.lgbt>
```

## Add images

You can add images that have been uploaded to the [image store](/images) using `![ ]( )`, where the `alt` text description of the image goes in the `[ ]` and the URL for the image goes in the `( )`. For example:

```
![The Civil Service LGBT+ Network wordmark](/assets/images/uploads/manuals/wordmark.jpg)
```

Images should appear on a new line, with a line break between the image link and other text.

## Blockquotes 

Blockquote text is highlighted separately from other text on the page. It is intended to draw attention to quotes or important information. There are two formats: regular and warning text.

### Regular blockquotes

Use regular block quotes for key information or to highlight a quote.

```
> This is text in a blockquote.
```

### Warning text

Use warning text for critical information that has severe consequences if the user fails to act.

```
{:.warning-text}
> **This is a warning.**
> 
> You should pay attention to this information.
```

## Tables

You can add tables by using the following format:

```
| Name       | Email address          |
|------------|------------------------|
| John       | john@civilservice.lgbt |
| Ash        | ash@civilservice.lgbt  |
````

## Horizontal rules

If you need to visually separate sections of a page, you can add a horizontal rule. Do this using three dashes on a separate line. For example

```
---
```

