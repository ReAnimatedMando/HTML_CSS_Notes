# HTML & CSS Notes

Much like a newspaper/word document, a web page is designed with headings, content, sub-headings, and more content to help direct the reader. **HTML** describes the structure of pages, and **CSS** styles that page. 

## HTML 

*    Elements of HTML live in angled brackets.
*    Elements are usually made up of two tags, an opening tag, and a closing tag. Notice the forward slash in the closing tag.
*    Basic elements and their meaning. HTML tags, anything between the open and close are part of the html. Body elements, anything between opening and closing should be shown inside the main browser window. h1 elements; words between are the main heading. p elements words between are a paragraph. h2 elements; words between are a sub-heading. 
*    Tags act like containers. They tell you something about the information that lies between their opening and closing tags. 
*    Attributes provide additional info about the contents of an element. They appear on the opening tag of the element and consist of a Name and a Value separated by =. p lang=”en-us”, Here the attribute lang is language and en-us specifies English-United States. Majority of attributes can only be used on certain elements. 
*    Before a body element (one shown within the web browser), you will often see a head element. This is info about the page (also known as meta data), often a title. head, title. - - Anything written between the title tags will appear in the title bar at the top of the browser window.  

## Headings

*   HTML has 6 levels of headings. h1 - h6
*   h1 elements are the largest and get smaller as you progress. Of course, you can control the size of text, as well as font, and color. This will be explored further in CSS.

## Paragraphs

*   p, by default, a browser will show each paragraph on a new line with some space between it and the subsequent paragraph

## Bold & Italic

*   Bold b, and Italic i.
*   Using these tags will make words enclosed in these elements appear bold or italic. 
*   b also represents a section of text that would be presented in a visually different way, such as key words in a paragraph.
*   i also represents a section of text that would be said in a different way from surrounding content, such as technical terms, names of ships, foreign words, thoughts, or other terms that would usually be italicized.

## Superscript & Subscript

*	sup or superscript examples are 4th and or 2 to the second power.
*	sub or subscript examples are CO2 as a chemical formula and footnotes.

## White Space

*	White space collapsing is what happens when a browser comes across 2 or more spaces next to each other and it automatically only displays 1 space.
*	Authors will take advantage of this to make their code easier to read. 

## Line Breaks & Horizontal Rules

*	br /, unlike when a p or h1 are shown on new lines, you can use br / to add a line break in the middle of a paragraph. 
*	To create a break between themes, such as a change of topic in a book, or a new scene in a play, you can add a horizontal rule using, hr /. 
*	These are also known as empty elements given that there are no words between an opening and closing tag. Hence, there is usually only one tag to an empty element and have a space before the slash, br /. 

## Semantic Markup

*	Some text elements are not intended to affect the structure of your web page, but instead add extra information to the page.
*	For example, the voice of a screen reader (accessibility is a requirement for all web pages), would know to emphasize certain words when the em element is used. Or a search engine would register the use of a quote if the blockquote element is used. 
*	Their purpose is to describe the content of your page more accurately. 

