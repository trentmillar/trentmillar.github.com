---
layout: post
title: "Markdown Cheat Sheet"
description: "Markdown Cheat Sheet"
category: "Coding"
tags: ['Markdown','Cheatsheet']
---
{% include JB/setup %}
My quick reference to the most commom MD. These examples are not pegged to Github markdown, instead I tried to cover what should be supported on all platforms.

## Block Elements

### Paragraphs & Breaks

To create a paragraph, simply create a block of text that is __not__ separated by one or more blank lines. Blocks of text separated by one or more blank lines will be parsed as paragraphs.

If you want to create a line break, end a line with two or more spaces, then hit Return/Enter.

_MD_\(dots are spaces in your MD\):

	This is a paragraph..
	This is just a continuing line of text
	This is also just a continuing line of text

_Results_:

This is a paragraph  
This is just a continuing line of text
This is also just a continuing line of text

---

### Headers

Markdown supports two header formats. The wiki editor uses the “atx’-style headers. Simply prefix your header text with the number of # characters to specify heading depth. For example: # H1, ## H2 and ### H3 will be progressively smaller headers, down to ###### H6.

_MD_:

	# H1
	## H2
	### H3
	#### H4
	##### H5
	###### H6

_Results_:

# H1
## H2
### H3
#### H4
##### H5
###### H6

---

### Blockquotes

Markdown creates blockquotes email-style by prefixing each line with the >. This looks best if you decide to hard-wrap text and prefix each line with a > character, but Markdown supports just putting > before your paragraph.

_MD_\(dots are spaces in your MD\):

	> This is a paragraph in a blockquote..  
	This is just a line
	I am also just a line

_Results_:

> This is a paragraph in a blockquote  
This is just a line
I am also just a line

---

### Lists

Markdown supports both ordered and unordered lists. To create an ordered list, simply prefix each line with a number (any number will do — this is why the editor only uses one number.) To create an unordered list, you can prefix each line with *, + or -.

_MD_:

	1. Apples
	2. Oranges

	* Potatoes
	* Carrots

_Results_:

1. Apples
2. Oranges

* Potatoes
* Carrots

List items can contain multiple paragraphs, however each paragraph must be indented by at least 4 spaces or a tab.

_MD_:

	1. Tree
		* Apples
		* Oranges
	2. Root
		* Potatoes
		* Carrots

_Results_:

1. Tree
	* Apples
	* Oranges
2. Root
	* Potatoes
	* Carrots

---

### Code Blocks

Markdown wraps code blocks in pre-formatted tags to preserve indentation in your code blocks. To create a code block, indent the entire block by at least 4 spaces or one tab. Markdown will strip the extra indentation you’ve added to the code block.

_MD_\(dots are spaces in your MD\):

	....class Button extends React.Components {
	....	render() {
	....		return <a className="btn">Click</a>
	....	}
	....}
	....window.App.Button = Button

_Results_:

	class Button extends React.Components {
		render() {
			return <a className="btn">Click</a>
		}
	}
	window.App.Button = Button

---

### Horizontal Rules

Horizontal rules are created by placing three or more hyphens, asterisks or underscores on a line by themselves. Spaces are allowed between the hyphens, asterisks or underscores.

_MD_:

	---

_Results_:

---   
   
   
---   

## Span Elements

### Links

Markdown has two types of links: inline and reference. For both types of links, the text you want to display to the user is placed in square brackets. For example, if you want your link to display the text “GitHub”, you write [GitHub].

To create an inline link, create a set of parentheses immediately after the brackets and write your URL within the parentheses. (e.g., [GitHub](https://github.com/)). Relative paths are allowed in inline links.

_MD_:

	[GitHub](https://github.com/)

_Results_:

[GitHub](https://github.com/)

---

### Emphasis

Asterisks (*) and underscores (_) are treated as emphasis and are wrapped with an <em> tag, which usually displays as italics in most browsers. Double asterisks (**) or double underscores (__) are treated as bold using the <strong> tag. To create italic or bold text, simply wrap your words in single/double asterisks/underscores. For example, **My double emphasis text** becomes My double emphasis text, and *My single emphasis text* becomes My single emphasis text.

_MD_:

	_italics_ __strong__ *italics* **strong**

_Results_:

_italics_ __strong__ *italics* **strong**

### Code

To create inline spans of code, simply wrap the code in backticks (\`). Markdown will turn `myFunction` into myFunction.

_MD_:

	`ReactDOM.render(<Button />, document.getElementById("container"))`

_Results_:

`ReactDOM.render(<Button />, document.getElementById("container"))`

### Images

Markdown image syntax looks a lot like the syntax for links; it is essentially the same syntax preceded by an exclamation point (!). For example, if you want to link to an image at https://github.com/unicorn.png with the alternate text My Unicorn, you would write \!\[My Unicorn\](https://github.com/unicorn.png).

_MD_:

	![My Unicorn](https://github.com/unicorn.png)

_Results_:

![My Unicorn](https://github.com/unicorn.png)

---

## Miscallaneous

### Automatic Links

If you want to create a link that displays the actual URL, markdown allows you to quickly wrap the URL in < and > to do so. For example, the link https://github.com/ is easily produced by writing \<https://github.com/\>.

_MD_:

	<https://github.com/>

_Results_:

<https://github.com/>	

### Escaping

If you want to use a special Markdown character in your document (such as displaying literal asterisks), you can escape the character with the backslash (\\). Markdown will ignore the character directly after a backslash.

_MD_:

	\_italics\_ \__strong\__

_Results_:

\_italics\_ \__strong\__

---	