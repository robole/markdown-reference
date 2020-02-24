# Markdown

Markdown is a simple markup langauge written in plain-text, which was designed to create documents that are easy to read and can be published on the internet (in HTML). Documents use a *.md* and *.markdown* file extension.

Mark Gruber wrote and released an informal specification through his [syntax description](https://daringfireball.net/projects/markdown/syntax) and a Perl script (*Markdown.pl*) in 2004. Markdown has been widely adopted since then, and it has become used in many other forms such as: readme documents, comments on forums, authoring of books, and slideshows. 

Since the initial specification of Markdown contained ambiguities and unanswered questions, the implementations that appeared over the years have subtle differences and many come with syntax extensions. 

## Philosophy

- Easy to read
- Easy to write
- Can publish as-is on the internet

>*The overriding design goal for Markdown’s formatting syntax is to make it as readable as possible. The idea is that a Markdown-formatted document should be publishable as-is, as plain text, without looking like it’s been marked up with tags or formatting instructions.* **- Mark Gruber**

## Standardization

There were different efforts to standardize implementations and form an offical standard, but none proved successful. In 2012, a group began an organised effort to form a standard, John Gruber objected to their plans, and eventually it became an alternative specification called [CommonMark](https://commonmark.org/), which is "a strongly defined, highly compatible specification of Markdown".

## Variant Specifications

- [CommonMark](https://commonmark.org/)
- [GitHub Flavored Markdown (GFM)](https://github.github.com/gfm): based on CommonMark.
- [Markdown Extra](https://michelf.ca/projects/php-markdown/extra/)
- [Multimarkdown](https://github.com/fletcher/MultiMarkdown)

## Syntax

Mostly Markdown is just regular text with a few special non-alphabetic characters thrown in such as \*.

### Paragraph

A paragraph is simply one or more consecutive lines of text, separated by one or more blank lines. 

### Headings

	# This is an <h1> tag
	## This is an <h2> tag
	### This is an <h3> tag
	#### This is an <h4> tag
	##### This is an <h5> tag
	###### This is an <h6> tag
	
### Emphasis

	*This text will be italic*
	_This will also be italic_

	**This text will be bold**
	__This will also be bold__

	_You **can** combine them_

### Unordered List

	* Item 1
	* Item 2
	  * Item 2a
	  * Item 2b

### Ordered List

	1. Item 1
	1. Item 2
	1. Item 3
	   1. Item 3a
	   1. Item 3b

### Images

	![logo](/images/logo.png)
	
Format: \!\[Alt Text\]\(url\)

### Links

	[Github](http://github.com)

Format: \[Link text\]\(url\)
	
Markdown supports a shortcut style for creating “automatic” links for URLs and email addresses: simply surround the URL or email address with angle brackets. 

Markdown will turn this:

	<http://example.com/>

into:

	<a href="http://example.com/">http://example.com/</a>


### Blockquotes

	> We're living the future so
	> the present is our past.

becomes this:

> We're living the future so 
> the present is our past.

### Code

Inline code is surrounded by backticks \`html\` like this: the `<html>` element is the root of all good.
	
Code blocks are indented by 4 spaces or a tab.

### Horizontal Rule

You can produce a horizontal rule (`<hr/>`) by placing three or more hyphens, asterisks, or underscores on a line by themselves. If you wish, you may use spaces between the hyphens or asterisks.

	* * *

	***

	*****

	- - -

	---------------------------------------


### Inline HTML

For any markup that is not covered by Markdown’s syntax, you can simply use HTML itself. 

### Backslash Escapes

You can use backslash escapes so tat characters which would otherwise have special meaning in Markdown’s formatting syntax make it into the outputted document. 

Markdown provides backslash escapes for the following characters:

	\   backslash
	`   backtick
	*   asterisk
	_   underscore
	{}  curly braces
	[]  square brackets
	()  parentheses
	#   hash mark
	+   plus sign
	-   minus sign (hyphen)
	.   dot
	!   exclamation mark
	
## Extended Markdown Features

TODO: add more here