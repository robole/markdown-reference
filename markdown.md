# Markdown

1. [What is it?](#what-is-it)
1. [Why use it?](#why-use-it)
1. [Specifications](#specifications)
1. [How do I use it?](#how-do-i-use-it)
1. [Syntax](#syntax)
1. [Extended Syntax](#extended-syntax)


# What is it?

Markdown is a minimal [markup langauge](https://en.wikipedia.org/wiki/Markup_language) to produce documents for the internet. Documents have a *.md* and *.markdown* file extension.

In 2004, John Gruber wrote and released the informal specification for Markdown. 
The motivation was to create a more eloquent alternative to writing in HTML, which can be tedious adding tags to "mark" every piece of content. Markdown has a simple syntax in plain text. 

### Philosophy

- Easy to write
- Easy to read
- Can be published as-is on the internet

>*The overriding design goal for Markdown’s formatting syntax is to make it as readable as possible. The idea is that a Markdown-formatted document should be publishable as-is, as plain text, without looking like it’s been marked up with tags or formatting instructions.* **- John Gruber**

## Why use it?

### It's widely used

It's become widely used in comment sections and for formatting messages on popular websites and apps such as: Reddit, Stack Overflow, OpenStreetMap, Github, Facebook, Whatsapp, and Slack.

It is used for building websites and blogs in tools like: Jekyll, Hugo, Github Pages, Squarespace, and others.

### Easy to learn

The syntax is short and simple to use. It is not that much different than plain text.

### Easy to convert to HTML and other formats

There are many different applications available to convert markdown to HTML and other formats reliably. 

### Use any text editor

Any text editor can be used.

### Portable format

It is a plain text format and is not tied to any Operating System or application.

## Specifications

In 2004, John Gruber wrote and released an informal specification with his [syntax description](https://daringfireball.net/projects/markdown/syntax) and a Perl script (*Markdown.pl*). The idea was that the markdown source file is parsed by the script and transformed into a HTML file to be published online. 

### Standardization

Markdown has been widely embraced and adopted. However, the initial specification of Markdown contained ambiguities and unanswered questions, and no complete de-facto standard has ever really existed, this has resulted in implementations having some subtle differences, and many now come have been extended with extra features. 

There were different efforts to standardize implementations and form an offical standard, but none proved successful. In 2012, a group began an organised effort to form a standard, John Gruber objected to their plans, and eventually it became an alternative specification called [CommonMark](https://commonmark.org/).

### Variant Specifications

- [CommonMark](https://commonmark.org/): A strongly defined, highly compatible specification of Markdown.
- [GitHub Flavored Markdown (GFM)](https://github.com/gfm): It is based on CommonMark, and supports syntax extensions such as: tables, task lists, autolinking, and strikethrough. It supports some specific features to github such as mentions.
- [Markdown Extra](https://michelf.ca/projects/php-markdown/extra/): This is an extension of markdown originally written in PHP but ported to other languages. It implements it's own specific set of amendments and extensions including: markdown inside HTML, definition lists, abbreviations, and footnotes. 


## How do I use it?

### Editor

To author and view a document there are many editors and plugins for applications available, they usually give you a live preview pane. Some give you [WYSIWYG](https://en.wikipedia.org/wiki/WYSIWYG) controls, special modes, document structure overview, and export options to generate the markdown into different formats. I will mention a few popular options here, this is not meant to be an exhaustive list!

![StackEdit screenshot](/img/stackedit-screenshot.jpg)

Online editors:
- [StackEdit](https://stackedit.io/app): StackEdit is a [WYSIWYG](https://en.wikipedia.org/wiki/WYSIWYG) style editor with excellent all-round markdown support. Its features include: the ability to sync and save files to third-party services (Google Drive, Dropbox), output to various file formats (HTML, PDF), configure style and metadata properties for files, and work offline. It is opensource. You must signup to use some features.
- [Dillinger](https://dillinger.io/): Dillinger has a minimalistic interface. Its features include: the ability to import files from various sources, save files to third-party services (Google Drive, Dropbox), and output to various file formats (HTML, Styled HTML, PDF). It is 100% opensource. It requires no signup.

Desktop editors:
- [IA Writer](https://ia.net/writer): Considered to be a “gold standard” for markdown editors. It's clean and easy to use, and designed to remove distractions so you can focus on the task at hand. It comes equipped with a preview option, focus mode, and custom keyboard shelf that keeps all your necessary tools and Markdown shortcuts close by. With loads of export options, iA Writer is an ideal choice for mobile writing. Available for Mac, Windows, iOS, and Android.
- [Typora](https://typora.io): Comprehensive and robust editor with syntax highlighting,support for advanced Markdown features such as mathematics and diagrams, and a wide range of export options. Typora automatically hides Markdown formatting, showing instead a preview of the final document. Available for Windows and Mac.

IDEs:
- [Atom](https://atom.io/): Provides a built-in side-by-side preview. Other plugins available.
- [Visual Code Studio](https://code.visualstudio.com/): Provides a built-in side-by-side preview. Other plugins available.

### Static Site Generators

[Jekyll](https://jekyllrb.com) and [Hugo](https://gohugo.io) will package your markdown files into a website. They both require some setup to organise your content to produce a website, but once you learn their way of doing things, it can be a productive way to create and maintain a website. This has become a popular trend, Github Pages uses Jekyll behind the scenes.

### Build Tools

Webpack, Gulp, and other build tools have markdown packages for integrating markdown related tasks into your build process.

### Command-line Tools

[Pandoc](https://github.com/jgm/pandoc) is popular to use on the command-line for bulk conversion.

## Syntax

Mostly Markdown is just plain text with a few special non-alphabetic characters such as \*, these mark that piece of text to be transformed, becoming some element in the HTML ouput.

### Paragraph

A paragraph is simply one or more consecutive lines of text, separated by one or more blank lines. 

### Headings

	# This is a Heading Level 1 (<h1>)
	## This is a Heading Level 2 (<h2>)
	### This is a Heading Level 3 (<h3>)
	#### This is a Heading Level 4 (<h4>)
	##### This is a Heading Level 5 (<h5>)
	###### This is a Heading Level 6 (<h6>)

To create a heading, add hashes in front of a word or phrase. The number of hashes corresponds to the heading level.

Alternative: you can use `==` for heading 1, `--` for heading 2. 


### Emphasis

	*This text will be italic*
	_This will also be italic_

	**This text will be bold**
	__This will also be bold__

	_You **can** combine them_
	
Asteriskes are preferred over underscores.

### Lists

#### Unordered List

	* Item 1
	* Item 2

Add asterisks (\*) in front of line items. 

To create a nested list, indent the list item by 4 spaces or a tab.

	* Item 1
	* Item 2
		* Item 2a
		* Item 2b
	 
Alternative: You can use a plus sign (/+) or hyphen (-) instead of an asterisk. You can also use these interchangeably.

#### Ordered List

	1. Item 1
	1. Item 2
	1. Item 3
	   1. Item 3a
	   1. Item 3b
	   
To create an ordered list, precede an item with a number followed by a dot. The numbers don’t have to be in numerical order, but the list should start with the number one.

To create a nested list, indent the list item by 4 spaces or a tab.

	1. Item 1
	1. Item 2
	1. Item 3
		1. Item 3a
		1. Item 3b

### Images

	![logo](/images/logo.png)
	
Format: *`![alternative text](URL)`*


### Links

	[Github](http://github.com)

Format: *`[link text\]\(url\)`*

#### Adding a title

To add a title, enclose it in parentheses after the URL.

	![logo](/images/logo.png "Go to home page")
	
### Shortcut style
	
Markdown supports a shortcut style for creating “automatic” links for URLs and email addresses: simply surround the URL or email address with angle brackets. 

Markdown will turn this: `<http://example.com/>` into this HTML: `<a href="http://example.com/">http://example.com/</a>`.

### Reference style

Reference-style links are there to improve readability. 

They are constructed in two parts: 

1. the part you keep inline with your text

   format: `[link text][label]`
   
1. the part you store separately somewhere in the file.

	format: `[label]: [URL] "title"`

For example:


	If you want to learn markdown, you cannot go wrong by reading [this tutorial][1]. Happy learning!

	[1]: https://github.com/robole/markdown-reference "Markdown Reference Repository"

The first part has a label in the second set of brackets, which you define yourself. It is not case sensitive and can include letters, numbers, spaces, or punctuation.

The second part of a reference-style link has the label in the first set of brackets, which matches the label from the first part. The title for the link can be enclosed in double quotes, single quotes, or parentheses.

You can place the second part of the link anywhere in the document. Some people place them immediately after the paragraph in which they appear while other people place them at the end of the document.


### Blockquotes

	> We're living the future so
	> the present is our past.

becomes this:

> We're living the future so 
> the present is our past.

### Code

Inline code is surrounded by backticks:

  \`html\` is the root of all good:

  becomes this: 

`<html>` is the root of all good.
	
Code blocks are indented by 4 spaces or a tab.

### Horizontal Rule

A horizontal rule is a line across the width of the page delinating the end of a section. You can produce a horizontal rule (`<hr/>`) by placing three or more hyphens, asterisks, or underscores on a line by themselves. If you wish, you may use spaces between the hyphens or asterisks.

	* * *

	***

	*****

	- - -

	---------------------------------------


### Inline HTML

For any markup that is not covered by Markdown’s syntax, you can simply use HTML itself. 

### Backslash Escapes

You can use backslash escapes so that you show the special markdown characters as plain text in your output. 

By wrting this `\*`, we can see this: \* .

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
	
## Extended Syntax

### Tables

You can create tables by using 3 or more hyphens (---) to create each column header, and by using pipes (|) to separate each column. 

	First Header | Second Header
	------------ | -------------
	Content from cell 1 | Content from cell 2
	Content in the first column | Content in the second column

becomes this:

First Header | Second Header
------------ | -------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

You can format the text within tables. For example, you can add links, code (words or phrases in backticks (\`) only, not code blocks), and emphasis.

You can’t add headings, blockquotes, lists, horizontal rules, images, or HTML tags inside a table.

Creating tables with hyphens and pipes can be tedious. To speed up the process, try using the [Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables).

### Fenced Code Blocks

Depending on the Markdown parser, you’ll use three backticks or three tildes (~) on the lines before and after the code block. 

You can specify syntax highlighting for the fenced code block by specifying a language next to the backticks before the fenced code block.

\`\`\`json
\{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
\}
\`\`\`

becomes this:

 ```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

### Autolinks

Many Markdown parsers will automatically turn URLs into links. That means if you type `http://www.example.com`, it will become a link.

You can disable this by using backticks.

### Footnotes

Footnotes are a concise way to link to additional notes that are placed at the bottom of the page. When you create a footnote, a superscript number with a link appears where you added the footnote reference. Readers can click the link to jump to the content.

To create a footnote reference, add a caret and an identifier inside brackets ([^1]). Identifiers can be numbers or words, but they can’t contain spaces or tabs.

	Here's a simple footnote,[^1].

	[^1]: This is my first footnote.

### Heading IDs

Adding custom IDs allows you to link directly to headings and modify them with CSS. To add a custom heading ID, enclose the custom ID in curly braces on the same line as the heading.

	### My Heading {custom-id}

becomes this:

	<h3 id="custom-id">My Heading</h3>

### Definition Lists

To create a definition list, type the term on the first line. On the next line, type a colon followed by a space and the definition.

	First Term
	: This is the definition of the first term.

becomes this:

	<dl>
	<dt>First Term</dt>
	<dd>This is the definition of the first term.</dd>
	</dl>

### Strikethrough

Add 2 tildes (~) before and after the words.

	~~The world is flat.~~

becomes this:

~~The world is flat.~~

### Task Lists

Task lists allow you to create a list of action items with checkboxes. 

To create a task list, add dashes and square brackets with a space in front of task list items. To select a checkbox, add an x in between the brackets, as below.

	- [x] Write the press release
	- [ ] Update the website
	- [ ] Contact the media

becomes this:

![task list](img/tasklist.png)

### Emoji

There are two ways to add emoji to Markdown files: copy and paste the emoji into your Markdown-formatted text, or type emoji shortcodes.

In most cases, you can simply copy an emoji from a source like [Emojipedia](https://emojipedia.org/), and paste it into your document. 

Some Markdown applications allow you to insert emoji by typing shortcodes. You surround the name of an emoji with colons.

	That is so funny! :joy:

becomes this:

That is so funny! :joy:

### Escape Characters

Also, the pipe character (|) can be escaped. This is included when tables are supported.