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

## Strong & Emphasis

*	The use of the strong element indicates the content has a strong importance and browsers will show these elements in bold lettering. 
*	The use of the em element shows a more subtle emphasis by showing the words in italics. 

## Quotations

*	There are two elements commonly used for marking up quotations. 
*	blockquote is used for longer quotes that take an entire paragraph. Note the a <p> element is still used in a blockquote element. Browsers tend to indent the contents of the blockquote element but you should not use it as an indent.
*	q is used for shorter quotes. Browsers are supposed to put “quotation” marks around these elements, however Internet Explorer does not so authors tend to avoid this tag. 
*	Both elements may use the cite attribute to indicate where the quote is from. Its value should be a URL that will have more information about the source. blockquote cite=http://en.wikipedia.org/wiki/Winnie-the-Pooh

## Abbreviations & Acronyms

*	abbr is used when you want to specify an abbreviation. For example, p abbr title=”professor”>Profabbrs.
*	Older verions of HTML included acronym, However abbr can now be used for both abbreviations and acronyms.

## Citations & Definitions

*	To reference a piece of work such as a book, journal, movie…. The cite element can be used. Browsers will render a cite element in italics. 
*	dfn or definition element is used when first explaining new terminology or concepts. Also known as its defining instance. The appearance of the dfn element is not always changed depending on the browser. p A dfnblack holedfn is a region of space from which nothing, not even light, can escape.p 

## Author Details

*	<address> elements contain contact details for the author of the page. This can be a physical address, email address, or phone number. Most browsers display this element in italics. 
*	Example: <address>
    -    pa href=mailto:homer@example.org
        homer@example.orgap
    -    p742 Evergreen Terrace, Springfield.p
    -    address     

## Changes to Content

*	ins Element is used to show content that has been inserted into a document and is rendered with the content underlined.
*	del Element is used to show content that has been deleted from a document and is rendered with a line through the content.
*	s Element is used when content is no longer relevant or accurate but should not be deleted and is rendered as having a line through the content contained in the element.

## Lists

*	Ordered lists are tagged ol and then each element in the list is tagged with its own li. They can be given an attribute to indicate the type of number, letter, roman numerals… but this is better styled using CSS. 
*	Unordered lists are tagged ul and like ordered lists each item is tagged lili. Also, like ordered lists, each item may be given an attribute to specify what type of bullet point (circle, squares, diamonds) … but again this is better stylized using CSS.
*	Definition lists are elements that usually consist of a series of terms and their definitions and are tagged dl. These Consist of both dt and dd elements, dt being the term that’s being defined, and dd being the definition of said term. 
*	Nested lists are sub lists that rest inside li elements such as the dark bullets followed by indented clear bullets used in the format of these notes. 

## Links

*	Types of links include from one website to another, from one page to another within the same website, from one part of a website to another, links to another browser window or tab, links that start up your email program and address a new email to someone else. 
*	Links are created using the a element. Example, 
a href=”http://www.imdb.com”>IMDB a. The last part of the element, IMDB, is the text the user sees and clicks on. This text should be user friendly, easy for users to know where the link is taking them.
*	Remember the a attribute element for a link will contain the href attribute and if you are directing them to a different website will need to contain the full web address. Browsers show links to websites in blue and underlined. 
*	Absolute and Relative URLS. URL stands for Uniform Resource Locator. Absolute URL starts with the domain name for that site and can be followed by the path to a specific page (.com). Relative URL is when you are linking to other pages within the same site (.html). They are a shorthand version of absolute URL.
*	On larger sites it is good practice to organize your code by placing the pages for each different section of the site into a new folder. Folders on a site are also referred to as directories (HTML&CSS pg. 82). 
    -	Relationships are used when referring to files and folders. The root folder (examplearts) is also the parent folder. The next group of sub-folders would be the children. The parent folder is also the grandparent folder to the sub-sub-folder, the grandchild. 
    -	The homepage of the site is index.html. So, the address to this site would be, www.examplearts.com/index.html. Within the index are the children, images, movies, music, and theater. The address to the logo for the site which sits in the images folder would be, examplearts.com/images/logo.gif. Grandchildren in this directory would be folders within movies, cinema, and dvd.
*	Email links open the users email program and addresses a specific email address. For these the href must include a mailto: attribute. 
a href=mailto:the_guma@yahoo.com>email Aaron/a.
*	When you want a link to open in a new window you use the target attribute. a href=http://www.imdb.com target=:blank” Internet movie database/a (opens in new window). Generally, this should be avoided, but when used, users should be notified.
*	When on a website that is one long page you may want to add links that direct users to lower down a page, midway, or back to top of the page. This saves users time from scrolling. You would do this by first adding id= to that particular part of the page in your html. Example, h1 id=”top”the first paragraph/h1. The link to this section would look like this… a href=”#top”>top/a
*	To link to a specific part of another page the technique is the same except you would precede the location with the absolute or relative URL.  
a href=”http://www.htmlcssbook.com/#bottom

## Images

*	Goals for IMG: Pick a format, display at correct size, optimize image for use on the web to make pages load faster. Images should also be relevant, convey information, be instantly recognizable, and fit the pages color palette. 
*	Images for a project should be well organized and be broken up into sub folders such as logos, banners, buttons, product photos … 
*	An img is empty so it has no closing tag. Within it must be a src= which tells the browser where it can find the image (usually a relative URL). Second it must contain a alt= which provides a description of the img. A title= attribute gives additional information about the img, and browsers can use this information to populate tooltips when the user hovers their cursor over the image. Alt text should give accurate information because the screen reader will use this for those with impairments. 
*	Height & Width of Images. These attributes within the element will specify the img height and width. This, however, is mostly done within CSS. 
*	Location of img within code can come before, inside the start, or in the middle of the p element. Remember that elements occupy their own line so an img before p would sit above that paragraph on its own line, one inside the start of p would be one the same line as the first paragraph line, and one within p would sit in the middle with the words on that line flowing around it. Images can also be aligned vertically, as well as left and right of words, but this only comes up in old code. 
*	3 golden rules to remember when creating images for your web page.
    -	Save the images in the right format: .jpeg, .gif, or .png. Failure to do so could result in poor image quality and it can also make the web page slower to load.
    -	Save images at the right size: You should have the image saved at the same width and height that you will have it displayed on your page. If it’s smaller, it will be distorted and stretched and if it’s bigger it will take longer to display on your page. Sizing images should be done well in a photo editor, and you should always think in terms of pixels. Images downloaded from the internet should be checked for size and more importantly, copyright. 
*	Image Formats
    -	.JPEG should be used when you have many different colors in a picture.
    -	.GIF & .PNG should be used when you have pictures that are flat and have large areas filled with the same color such as logos, illustrations, and diagrams. 
        *	Note that pictures of snow, sky, or grass are not flat and contain many colors, therefore should be formatted .JPEG.
*	Vector images are line drawings such as logos, illustrations, and diagrams, created in software such as Adobe Illustrator and can be resized without affecting quality. 
*	Animated GIFs can be created in photoshop and included in your web page, but this adds to file size and can slow downloading which should be avoided. 
*	Transparent images can also be used as either straight (GIF), or diagonal, round, semi-opaque, drop-shadow. (PNG)
*	Figure and figure caption: Add images with a caption by using the figure element which will contain your img info and caption all in one element. figcaption can be used to add a caption to an existing element. 

## Tables

*	When presenting information in tables you need to think in terms of a grid made up of rows and columns. 
*	Basic table structure - table element is used to create the table and the contents of that table are written row by row. tr stands for table row. Within it is the element td or table data, there is one td for each row and ended with /tr before starting the next tr or row.  
*	The th or table heading element is like td but instead represents the headings of each row or column. th can be used with a scope= element to indicate if it is a column or row. 
th scope=”col”>Saturday /th 
*	Sometimes you may need entries in a table to stretch across more than one column. This is called spanning columns. This is done using a colspan attribute and can be applied to a td or th element. Adding a number to a colspan attribute will determine how many columns it spans. td colspan=”2”>Geography /td will make geography span 2 columns. The same can be done for rows using the rowspan= attribute. td rowspan=”2”>movie /td
*	Long tables like long pages can contain headers and footers to help distinguish between elements in the table that may differ. These elements are thead, tbody, and tfoot. 

## Forms

*	Like a hard copy form that someone would fill out to provide you with information, a form on your website aims to collect data from your visitors. These forms include but are not limited to, search boxes, subscription buttons, and multiple-choice options. 
*	To differentiate between inputted data, information is traded from the browser to the server using name/value pairs. If the form allows text input, the name would be the username box, and the value would be the name entered by the user. If the form is multiple choice button based, the vote would be the name and the button selected, “Herbie”, would be the value. 
*	form elements always carry action= attributes. Its value is the URL for the page on the server that will receive the information in the form when submitted. 
*	input element is used to create several different form controls. The type= attribute determines if the form is text, radio, checkbox, submit, file etc. When users enter information, the server needs to know which form controls each piece of data that was entered. i.e. what’s been entered a username or a password? Maxlength= attribute can be used to set a limit of what a user is able to enter into a text box. 
*	When a type= element has a value of “password”, the box acts the same as a text box, but knows to block out the le****s. 
*	textarea element is used to create multi-line text input. This is used for comment boxes etc. 
*	Type=”radio” buttons allow users to pick one of a few options. Here the name= attribute should be the same for all options, the value= attribute indicates the value that is chosen and sent back to the server, and each should differ. A checked= attribute can be used to load the form with one, if any, values already checked. Radio buttons cannot be deselected, and this should be noted, if you want deselect as an option you should use a checkbox. 
*	Type=”checkbox” allow users to select and deselect one or more options. Like radio, name= is sent to the server with the value of the options the user selects and should be uniform across elements. value= is unique naming the box the user selects. checked= determines which, if any, boxes should load checked. 
*	select elements are used for dropdown lists. They contain 2 or more options the option element names these with value= attributes. To create a box that gives users the ability to select multiple options, the attribute of multiple= is added to the select element. 
*	When allowing users to upload files input type=”file” name=”user-song” /, the form element must have a value of “post”, instead of “get”. 
*	input type=”submit” is used to send a form to the server. name= is used to name attribute. value= controls the text that appears on the button. If you want to use an image for the subscribe button, you can use value= to link an image in the input element. button> elements give users more control over how their buttons appear. 
*	Each form control should be given its own label using label> elements after the input>. This can be put ahead of the input, or after, separating the radio button from its label. This is given the for=”” attribute which coincides with the id=”” within the input. 
*	fieldset> can be used for longer forms that contain more information. This groups them similarly to tables. legend> is used to caption and identify the purpose of the fieldset.
*	Required= is HTML5 version of form validation. This makes it so validation happen within the browser and saves time spent on server validation. 
*	Email, dates, and search boxes can also be created using input> by simply changing the type=”” attribute to “search”, “email”, or “date”. 

## Comments, Attributes, & more

*	Be aware of older versions of HTML (HTML4, XHTML 1.0, XML), so that you are aware of what features won’t be available to some users due to outdated browsers. 
*	octype html>. Doctypes were created to include in your meta data in order to specify what version of HTML you are using. This can help in the web page being rendered correctly. 
*	Comments can be added to code using !-- -->. Comments using this element are not visible by users and can help authors and collaborators understand the code. Comments are also helpful if the author wants to make a note to add something later but doesn’t yet have the file needed. For example, <-- add link here --> 
*	ID attributes can be added to any element and will give that element a unique identifier that can be targeted when styling with CSS. Any id given must be entirely unique to that element, possessed by none other on the page. 
*	Class attributes are other identifiers that can be given to many elements. In other words, many elements can be given a class as class=”important”. This is another attribute that would correlate to a command given in CSS. 
*	Block elements are elements that will always appear to start on a new line. i.e. h1>, p>, ul>, and li>.
*	Inline elements will always appear to continue on the same line. i.e. a>, b>, em>, and img>. 
*	div> or divisions help group sets of elements together in one block-level box. This helps in styling and organization. Since div> hold many elements within it, it is wise to add comments to tell yourself and others what division that code belongs to. For example, you would make a header division (for title and logo), or a comment section division (for users to leave comments). 
*	Span or span> is the inline element that contains text you want to differentiate from the rest of the paragraph and can be identified and styled with CSS. 
*	Iframes or iframe> are windows cut into your page. An example of this would be an embedded google map. To structure an iframe> you will need to know info for the attributes, src=”http://google.maps”, height=”350”, and width=”450”. 
*	Meta data lives in the head> of your page and is not visible to users. It is simply information about your code such as description, keywords, author info, pragma (keeps browser from caching page), expires (notes when page should no longer be cached). 

## Intro to CSS

*	CSS or Cascading Style Sheets – allows you to create rules that specify how the content of an element should appear. One key to understanding CSS is to imagine that there is an invisible box around every HTML element. Remember that you can assign each element in your HTML a unique identifier that will help CSS determine what elements to apply your chosen styles to. 
    -	A CSS rule contains two parts: a selector and a declaration. 
    	*A selector indicates which element the rule applies to.
	    A declaration indicates how that element should be styled. Declarations are split into two parts: the property and the value. The property is the aspect of the element you want to change, i.e. color, font, width, height, and border. The value specify the settings for the given property, i.e. for a property of color the value could be blue. You can specify multiple properties in one declaration by separating each with a semi-colon.

## Internal & External CSS

*	External CSS means you are using a file separate the HTML file and must create a link within your HTML to your CSS. The CSS link lives inside the <head> of your HTML and uses 3 attributes. 
    -	Href=”” – Specifies the path to the file with is often a css or styles folder. 
    -	Type=”” – Specifies the type of document which is “text/css”.
    -	Rel=”” – Specifies relationship between the HTML page and the linked file. Should always be a stylesheet.
        *	An HTML page can use and be linked to multiple CSS style sheets. This can help when you want to specify one stylesheet for layout and another for presentation. 
*	Internal CSS means you can also add CSS rules within your HTML page by using the <style> element. This needs a type=”” attribute of text/css. However, this method is only seen in older code and is not recommended because…
    -	The code must be repeated for each element because it does not cascade. This is particularly bad when making multiple pages.
    -	It also keeps the content separate from how the page looks. 
    -	You cannot change across all pages and would have to make changes to each individual element on each page. 

## CSS Selectors

*	Universal selector – Apply to all elements in document. * {}
*	Type selector – Matches element names. H1, h2, h3 {}
*	Class selector – Matches an element whose class attribute has a value that matches the one specified after the period or full stop symbol. .note {} – targets element whose class attribute has a value of note. P.note {} – targets only p> element whose class attribute has a value of note. p class=”note” />
*	ID selector – Matches an element whose id attribute has a value that matches the one specified after the pound or hash symbol. #introduction {} – targets the element whose id attribute has a value of introduction. h1 id=”introduction” />
*	Child selector – Matches an element that is a direct child of another. Li>a {} – targets any a> element that are children of another li> element but no other a> elements on that page. 
*	Descendant selector – Matches an element that is a descendant of another specified element not just a direct child of that element. P a {} – targets any a> elements that sit inside a p> element, even if there are other elements nested between. 
*	Adjacent sibling selector – Matches an element that is the next sibling of another. H1+p {} – targets the first p> element after any h1> element but not other p> elements.
*	General sibling selector – Matches an element that is a sibling of another, although it does not have to be the directly preceding element. H1~p {} – if you had two p> elements that are siblings of an h1> element, this rule would apply to both. 

## CSS Cascade

*	CSS rules and how they cascade – If two or more rules apply to the same element there are ways to determine which will take precedence. 
    -	Last rule – if the two selectors are identical, the latter will take precedence over the former. 
    -	Specificity – The more specific rule will take precedence, i.e. p b is more specific than p.
    -	Important – Labeling and property or value !important will make it more important than any other rule. Good for making changes to a single element after cascading general rules to make clean code. 
*	Inheritance – In the instance of font, you can specify the font-family or color properties on the body> element and they will apply to most child elements. You can also force a lot of properties to inherit values from their parent elements by using inherit for the value of properties, i.e. padding: inherit; 
    -	PG. 242 for resources

## Color in CSS

*	Foreground color – Color properties can be expressed in 3 ways.
    -	RGB value – rgb(100,100,90)
    -	Hex codes – Preceded by a #, these 6-digit codes represent the amount of red, green, and blue in a color. #ee3e80.
    -	Color Names – There are 147 color names that are recognized by browsers such as DarkCyan. 
        *	It is not necessary to memorize these designations. 
        *	/* comments in these symbols like in HTML are not visible to users and can help authors and collaborators understand your code */
*	Background color – CSS treats HTML elements as if they’re in a box and the background-color property sets the background color for that box. i.e. body { background-color: DarkCyan;}. 
    -	Color picking tools such as the ones found in photoshop, contain the RGB values as well as the #fcc00 hex code numbers for each color you highlight. 
*	When picking background and foreground colors, it is imperative that you ensure that there is enough contrast for the text to be legible. A high contrast makes it easier for users to see text. For long spans of text, medium contrast can help with readability. 
*	Opacity – a value given to a color with a number between 0.0 and 1.0, translating to 0%-100% opacity. i.e. background color: rgba(0,0,0,0.5), here the a is the opacity. 
*	Hue, saturation, and lightness are also features you can apply to your css. i.e. background color: #c8c8c8; background color: hsla(0,100%,100%,0.5). Once again, the a in this code represents the a as being opacity. 

## Text

*	Properties that control the appearance of text can be split into two groups.
    -	Those that directly affect the font and its appearance.
    -	Those that would have the same effect on text no matter what font you were using, including color and spacing between words and letters. 
*	Typeface terms:
    -	Serif – fonts have extra details on the ends of the main strokes of letters.
    -	Sans-serif - fonts have straight ends to letters and are a much cleaner design. 
    -	Monospace – Every letter is the same width. They align nicely and are used commonly in code. 
    -	Weight – Font weight not only adds emphasis but can also affect the amount of white space and contrast on a page. 
    -	Style – Italic fonts have a cursive aspect and Oblique fonts take the normal style and put it at an angle. 
    -	Stretch – In condensed versions of the font, letters are thinner and closer together. In expanded versions they are thicker and further apart. 
*	When choosing a typeface/font, it is important to understand that the browser will usually only display it if it’s installed on that user’s computer. So, sites often use a small set of typefaces that are installed on most computers. More than one can be specified in your code to act as backups. This is known as a font-family as is typed in HTML like font-family: Georgia, Times, Serif; 
*	Font type scales are as follows:
    -	Pixels – best way to size your text. Pixels are relative to the resolution of the screen, so the same type size will look larger on a higher resolution screen. 
    -	Percentages – Default text size of a browser is 16. Using percentages of this amount gives you relatively larger and smaller text size. 
    -	Ems – Similar to percentages. 
*	Font-family limits you to the fonts available on users’ computers. @font-face allows you to use a font even if it is not installed on users’ computers. It does this by allowing you to specify a path to a copy of the font which will be downloaded to the user’s computer, so it is important that the font licensing allows it to be used in this way. 
*	Text-transform – Used to change the case of text giving it one of three values.
    -	Uppercase – text-transform: uppercase;
    -	Lowercase
    -	Capitalize
*	Text-decoration – allows you to specify the following values.
    -	None – removes any already applied
    -	Underline
    -	Overline
    -	Line-through
    -	Blink – animates text to make it flash on and off. 
*	Line-height – leading is a term for vertical space between lines of text. It is measured from the bottom of the descender on one line to the top of the ascender on the next line. 
    -	Descender – part of a letter that drops below the baseline.
    -	ascender – highest point of a letter.
*	Letter-spacing, word-spacing – kerning is the term for the space between each letter. Word spacing and letter spacing, and line height should be measured in em. 
*	Text-align – allows control of alignment of text.
    -	Left
    -	Right
    -	Center
    -	Justify – every line in a paragraph, except the last line, should be set to take up the full width of the containing box. 
*	Vertical-align – aligns relative to an image or box.
    -	Baseline
    -	Sub
    -	Super
    -	Top
    -	Middle
    -	Bottom
*	Text-indent – allows you to indent the first line of text within an element. 
*	Text-shadow – used to create a dropshadow.
    -	Requires 3 lengths and a color as a value. i.e. 2px 2px 7px #111111. First length is how far to the left or right the shadow falls. Second length is distance top or bottom shadow should fall. Third length is optional and controls blur. Fourth is the color of the drop shadow. 
    -	:first-letter, :first-line – can be used to add values to selected elements such as weight, style, size. 
*	:link, :visited – browsers tend to show links in blue with an underline by default, and they will change colors of the links that have been visited. 
    -	:link – allows you to set styles for links.
    -	:visited – allows you to set styles for links that have been clicked on. 
*	:hover, :active, :focus – pseudo classes that allow you to change the appearance of elements when a user is interacting with them.
    -	:hover – Styles links and buttons when a user is hovering over them with a cursor. 
    -	:active - Styles links and buttons when a user clicks on them to make them feel more interactive. 
    -	:focus – Focus occurs when a browser discovers that you are ready to interact, i.e. when your cursor is in a form input ready to accept typing. 
        *	Pseudo-classes should appear in this order.
            -	:link, :visited, :hover, :focus, :active
*	Attribute Selectors:
    -	Pclass] – targets any p> element with an attribute called class. 
    -	Pclass=”dog”] – targets any p> element with an attribute called class whose value is dog.
    -	Pclass~=”dog”] – targets p> element with an attribute called class whose value is a list of space-separated words, one of which is dog.
    -	Pattr^”d”] – targets any p> element with an attribute whose value begins with the letter “d”.
    -	[attr*”do”] – targets any p> element with an attribute whose value contains the letters “do”.
    -	Pattr$”g”] – targets any p> element with an attribute whose value ends with the letter “g”.

## Borders

*	Remember that your boxes are your elements, i.e. your p>, h>, and div>… In CSS you can style each of these with the use of the following properties. 
*	Height and width. Measured in px, %, or em. You can set a div> to be 300px height and 400px width and then set a p> within it to be 75% h and w and that p> will be that percentage of the div>.
*	Limiting width with min-width, and max-width. This is so your page design will shrink and expand to fit the size of the users screen. 
*	Limiting height with min-height and max-height. Same idea as width. 
*	Overflow – Tells the browser what to do if the content contained within a box is larger than the box itself. 
    -	Hidden – simply hides extra content that doesn’t fit in the box. 
    -	Scroll- adds a scrollbar to the box so users can scroll to see the missing content. 
*	Every box has three properties that can be adjusted to control its appearance.
    -	Border – The border separates the edge of one box from another. Every box has a border visible or not. 
    -	Margin – Sit outside the edge of the border and can be set to create a gap between the borders of two adjacent boxes. 
    -	Padding – The space between the border of a box and any content contained within it. Can increase readability. 
*	Border:
    -	Border-width; value can be px or thin, medium, thick. You can control  individual size of borders using, border-top, border-right, border-bottom, border-left-width, i.e. border width: 2px 1px 1px 2px, and always goes top, right, bottom, left. 
    -	Border-style; values.
        *	Solid – a single solid line.
        *	Dotted – series of square dots.
        *	Dashed – series of short lines.
        *	Double – two solid lines.
        *	Groove – appears to be carved into page.
        *	Ridge – appears to stick out from page.
        *	Inset – appears to be embedded.
        *	Outset – looks like it is coming out of screen.
        *	Hidden/none – no border shown. 
*	Can be individually styled top, left, right, bottom. 
    -	Border-color – borders can be colored as a whole or individually using border-top, right, bottom, left-color. 
    -	Shorthand border: 3px dotted #0088dd/darkcyan. Size, type, and color. 
    -	Padding - How much space appears between  the content of an element and its border. Measured in px, %, or em. Can specify different values for top, right, bottom, and left. 
    -	Margin – Controls gap between boxes. Measured in px, %, or em. Can specify different values for top, right, bottom, and left. 
    -	Centering content – Box width must be set to center content. Setting left and right margins to auto will place the box an equal distance away on each side. Text-align should be set as you want it as it will inherit the parent properties. 
    -	Changing inline/block. Display – allows you to turn an inline element into a block-level element or vice-versa. 
        *	Inline – cause a block-level element to act like an inline element. 
        *	Block – cause an inline element to act like a block-level element. 
        *	Inline-block- combination
        *	None – hides an element from the page. 
*	block-level elements will sit side by side rather than starting on new lines. 
    -	Visibility – self explanatory
*	Hidden 
*	Visible 
    -	Border-image – takes a background image and slices it into nine pieces. 
        *	Requires three pieces of information.
*	URL of the image
*	Where to slice image
*	What to do with straight edges
    -	Stretch
    -	Repeat
    -	Round
    -	Box-shadow – allows you to add drop shadow around a box. Works just like text shadow. Must use at least the first two of following values and a color. 
        *	Horizontal offset – negative values position the shadow to the left of the box.
        *	Vertical offset – negative values position shadow to the top of the box.
        *	Blur distance – if omitted, the shadow is a solid line like a border.
        *	Spread of shadow – if used, a positive value will cause the shadow to expand in all directions, and a negative value will make it contract. 
*	Inset can be used to create an inner shadow. 
    -	i.e. box-shadow: 0 0 10px #gray
        *	HO VO BD SOS
    -	Border-radius – Allows you to create rounded corners. Can be individually specified top-right, bottom-right, bottom-left, top-left. 
        *	Can use to create complex shapes using multiple values per radius. i.e. top-right: 80px 50px.

## Lists, Tables, & Forms

*	list-style-type – Allows you to control the shape or style of a bullet point/marker. Applies to <ol>, <ul>, & <li>.
    -	For <ul> you can use….
        *	None, disc, circle, or square.
    -	For <ol> you can use…
        *	Decimal, decimal-leading-zero, lower-alpha, upper-alpha, lower-roman, upper-roman. 
*	list-style-image – you can also specify an image to act as a bullet point using an image. list-style-image: url(“images/star.png”);
*	list-style-position – Lists are indented into the page by default. This property indicates whether the marker should be on the inside or the outside of the box containing the main points. List-style-position: outside; list-style-position: inside;
*	list-style – Shorthand, list-style: allows you to express the markers’ style, image, and position in any order. 
*	Table Properties:
    -	Width – sets width of table.
    -	Padding – to set the space between the border of each table call and its content. 
    -	Text-transform – to convert the content of the table headers to uppercase. 
    -	Letter-spacing, font-size – to add additional styling to the content of the table headers. 
    -	Border-top, border-bottom – to set borders above and below the table headers. 
    -	Text-align – to align the writing to the left of some table cells and to the right of the others. 
    -	Background-color – to change the background color of the alternating rows.
    -	.hover – to highlight a table row when a user’s mouse goes over it. 
*	Property tips:
    -	Give cells padding – adding padding helps improve readability.
    -	Distinguish headings – Style in bold, make uppercase, underline, and add a background color to distinguish headings. 
    -	Shade alternate rows – shading every other row can help users follow along the lines. 
    -	Align numerals – you can use text-align to align content of any column that contains numbers to the right.
*	Empty-cells – you can use this property to specify if you want the borders of empty cells to be shown.
    -	Empty-cells: show; or empty-cells: hide;
    -	Inherit can be used if you have one table nested inside another.
*	Border-spacing, border-collapse:
    -	 Collapse – borders are collapsed into a single border where possible.
    -	Separate – Borders are detached from each other and given space that is specified… 5px 15px.

## Styling Forms

* Styling forms to make them easier and maybe even more fun to use is a great way to attract users. Common elements to style include.
*	Text inputs and text areas.
*	Submit buttons.
*	Labels on forms to get the form controls to align nicely. 

## Styling Text Inputs

*Styling text buttons
    -	Font-size – Sets size of text entered by user.
    -	Color & background color – sets text color and sets background color of the input. 
    -	Border – adds a border around the edge of the input box.
    -	Border-radius – can be used to create rounded corners.
    -	:focus – pseudo-class is used to change the background color of the text input when it is being used. 
    -	:hover – pseudo-class applies the same styles when the user hovers over inputs.
    -	Background image – adds a background image to the box. Because there is a different image for each input, we are using an attribute selector looking for the value of the id attribute on each input. 
*	Styling submit buttons
    -	Color – used to change the color of the text on the button.
    -	Text-shadow – can give a 3d look to the text in browsers that support the property.
    -	Border-bottom – had been used to make the bottom border of the button slightly thicker to give it a 3d feel. 
    -	Background-color – can make the button stand out. Being consistent with colors and styles across pages can help users learn to navigate your pages more easily. 
    -	:hover – pseudo-class used to change the buttons appearance when users hover over it. 
*	Fieldsets and legends – Helpful in determining the edges of a form. In a long form they can help group together related information within it. Legends are used to indicate what information is required in the fieldset. Properties commonly used with these two elements are…
    -	Width
    -	Color
    -	Background-color
    -	Border
    -	Border-radius
    -	Padding
*	Cursor – allows you control over the type of mouse cursor that should be displayed to users. Commonly used values are…
    -	Auto
    -	Crosshair
    -	Default
    -	Pointer
    -	Move
    -	Text
    -	Wait
    -	Help
    -	url(“cursor.gif”); 

## Layout

* Controlling position of elements, creating site layouts, designing for different sized screens.
*	Building blocks – CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline-box.
    -	Block-level elements – start on a new line.
        *	h1>
        *	p>
        *	ul>
        *	li>
    -	Inline elements – Flow between surrounding text.
        *	img>
        *	b>
        *	i>
*	Containing elements – If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.
    -	It is common to group a number of elements together inside a div> (or other block-level) element. These div> elements could be the header, main content, or the footer, and are all contained in the body>. 
        *	A box may be nested inside several other block-level elements. The containing element is always the direct parent of that element. 
*	Controlling the position of elements – CSS has positioning schemes that allow you to control the layout of a page. 
    -	Normal flow – Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one. This is the default behavior unless otherwise specified. One after the other, vertically down the page. 
        *	position:static. Since this is the default way browsers treat HTML elements, you do not need a CSS property.
    -	Relative positioning – This moves the element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed. This does not affect the position of surrounding elements; they stay in the position they would be in normal flow. 
        *	position:relative. You can move an element anywhere in relation to where it would be in normal flow. 10px lower, 20% to the right. Top, bottom, left, or right are the properties you would use to offset the element. 
    -	Absolute positioning – This positions the element in relation to its containing element. It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they ignore the space it would have taken up). Absolutely positioned elements move as users scroll up and down the page. 
        *	position:absolute. Properties are top, bottom, left, or right. You can separate a heading by setting it 500px left with width of 250px and setting width of the paragraph at 450px. These elements will not overlap. 
    -	Fixed positioning – This is a form of absolute positioning that positions the element I relation to the browser window, as opposed to the containing element. Elements with fixed positioning do not affect the position of surrounding elements and they do not move when the user scrolls up or down. 
        *	position:fixed. Using margin for the p> is good to start the p> below where the h1> is fixed so that it won’t overlap at the top.
    -	Floating elements – Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow. 
        *	float. Always use the width property with float. This is great for adding blockquote> element to p> and having it sit to the right or left of the p>.  
        *	Float can be used to place boxes (p>), next to each other. 
        *	.clear property allows you to say that no element (within the same containing element), should touch the left or right-hand sides of a box. The values can be left, right, both, and none. .clear properties require a class=”clear” in its HTML id.  Page 372
        *	Parents of floated elements problem. If a containing element only contains floated elements, some browsers will treat it as if it is 0px. Causing border properties to disappear. This is solved with the overflow and width properties in CSS. So, to a border you would add { border: 1px solid #665544; overflow: auto; width: 100%;
        *	Multi-column layouts are achieved with div> representing each column and each given a corresponding class. div class=”column1of2”> the CSS being .column1of2 and having the properties of width, float, and margin.
*	Width sets width of identified columns.
*	Float positions the columns next to each other.
*	Margin creates a gap between the columns.
    -	When you move any element from normal flow, boxes can overlap. The z-index property allows you to control which box appears on top.
*	Place z-index property in the element you want to sit on top. The element with a z-index of the highest number will take priority over elements with z-indexes of a lower number.
*	Screen sizes – Your design needs to be able to work on a range of different sized screens. 
    -	resolution – refers to the number of dots a screen shows per inch. Resolutions change according to users. 
        *	Iphone 4 – size=3.4 inches, resolution=960 x 640 px
        *	Ipad 2 – size=9.7”, resolution=1024 x 768 px
        *	13” Macbook – size=13.3”, resolution=1280 x 800 px
        *	27” iMac – size=27”, resolution=2560 x 1440 px
    -	Page sizes – designers try to stay in a range of 960 x 1000 px wide. Most users will be able to see designs this wide. Because of the wide range of screen sizes, designers know that some users will need to scroll, and are likely to do so if interested in the content. However, it is still wise to design your page to show interest in the first 570-600 px and entice scrolling with teases towards the bottom of this range. 
*	Fixed width layouts – do not change size as the user increases or decreases the size of their window.
    -	Advantages
        *	Px values are accurate at controlling size and positioning of elements.
        *	Designer has greater control over appearance and position of items on the page.
        *	Can control the lengths of lines and of text regardless of the size of user’s window.
        *	The size of an image will always remain the same relative to the rest of the page.
    -	Disadvantages
        *	You can end up with big gaps around the edge of a page.
        *	If user resolution is much higher the page can look smaller and be hard to read. 
        *	If user increases font size, text might not fit into designated spaces. 
        *	Design works best on devices that have a site or resolution similar to that of the desktop or laptop.
        *	Page will often take up more vertical space than a liquid layout with the same content. 
*	Liquid layout – designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages. 
    -	Advantages
        *	Pages expand to fill the entire browser window so there are no spaces around the page on a larger screen.
        *	Page can contract to fit users’ smaller windows without them having to scroll to the side. 
        *	Design is tolerant of users setting font sizes larger than the designer intended.
    -	Disadvantages
        *	Must control width of sections or the design can look very different than intended with gaps or squashing. 
        *	If user has a wide window, lines of text can become very long, making them hard to read. 
        *	If user has a narrow window, lines of text can become squashed, and few words will occupy a line. 
        *	Fixed items like images can be overflow into text if the window is made too small by the user. 
*	Some of these issues can be solved by giving some elements max and min widths while others will be allowed to be liquid. 
*	Layout Grids – Composition is the placement or arrangement of visual elements/how they are organized on a page. Designers use grid structures to help them position items on a page. Grids set consistent proportions and spaces between items which helps to create professional looking designs. 
    -	Grids create continuity between different pages which may use different designs.
    -	Help users predict where to find information on various pages.
    -	Make it easier to add new content to the site in a consistent way.
    -	Helps people collaborate on the design of a site in a consistent way. 
        *	Examples of possible layouts on page 389-392.
    -	CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions	of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch. 
*	Multiple Style Sheets – Some web page authors split their CSS style rules into separate style sheets. For example, they might use one to control the layout and another to control fonts, colors and so on. Some authors take an even more modular approach to stylesheets, creating separate stylesheets to control typography, layout, forms, tables, even different styles for each sub-section of a site. 
    -	There are two ways to add multiple style sheets to a page.
        *	Your HTML page can link to one style sheet and that stylesheet can use the @import rule to import other style sheets.
*	If a stylesheet uses the @import rule, it should appear before the other rules. 
    -	In the HTML you can use a separate link> element for each stylesheet. 
*	This link> always goes in the head> element of your HTML. 

## Images

*   Controlling size of images in CSS, aligning images in CSS, adding background images. 
*	Control image size using the width and height properties in CSS. Specifying image size in CSS will help your page load faster. Being consistent with your image sizes is very helpful. Having your product images match, as well as banners, featured photos, etc. Some ranges include small portrait – 220x360, small landscape – 330x210, and feature – 620x400. When designing your site, you should first determine the sizes of images that will be used and give each size a name such as, small, medium, and large. These sizes can be used in the class= element of your html in place of width and height and will later be specified in your CSS. PAGE; 409. 
*	Aligning images – You can use the float property to align images. You can add an align-left or right to your class in HTML as well as the size identifier, i.e. class=”align-right medium”; It is also a good idea to add a margin to the image so that it doesn’t touch the text around it. 
*	Centering images – by default, images are inline elements. This is changed by turning it into a block-level element by using the display property in CSS to be able to center the image. Once your image is set to display: block; it can be centered using the text-align property and giving it a value of center. 
*	Background-image – Background images can be placed behind any HTML and cover the entire background or just parts/grids/blocks. This is achieved using the background-image: property with a value that is a URL(“images/folder.gif”). Adding this property to the body will cover the entire background, and adding it to a p or paragraph will only cover that block. 
*	Repeating images – The background-repeat can have four values.
    -	Repeat – the background image is repeated both horizontally and vertically. Default
    -	Repeat-x – the image is repeated horizontally only.
    -	Repeat-y - the image is repeated vertically only.
    -	No-repeat – the image is only shown once.
*	Background-attachment – property specifies whether a background image should stay in one position or move as the user scrolls up or down the page. It can have one of two values.
    -	Fixed – the background image stays in the same position on the page.
    -	Scroll – the background image moves up and down as the user scrolls up and down the page. 
*	background-position – When not being repeated, you can use the background position property to specify where in the browser window the background image should be placed. This property usually has two values, the first represents the horizontal position and the second represents the vertical position. i.e. left top, left center, left bottom, right top, center center. Only specifying one value will result in the second value defaulting to center. Percentages and pixels can also be used for more exact positions in relation to the edges of the page. 
*	Background shorthand will show in this order
    -	Background-color
    -	Background-image
    -	Background-repeat
    -	Background-attachment
    -	background-position
        *	i.e. div {
*	background: #ffffff url(“”) no-repeat top right
*	Image rollovers & Sprites – Using CSS it is possible to create a link or button that changes to a second style when a user moves their mouse over it(known as rollover) and a third style when they click on it. This can be done by setting a background image for the link or button that has three different styles of the same button but only allows enough space to show one of them at a time. 
    -	Sprites are when a single image is used for different parts of the interface. Can make loading faster. 
    -	Page 417-18
*	CSS gradients – background-image and then specify the two colors that the gradient falls between. 
*	If you want to overlay text on a background image, the image must be low contrast in order for the text to be legible. 

## New HTML5 elements

*   Using class or id attributes to indicate the role of a div> element in the structure of a page is commonplace. However, HTML5 has introduced a new set of elements that allow you to divide up the parts of a page. The names of these elements indicate the kind of content you will find in them. Some of these elements are. 
*	header>, nav>, article>, aside>, footer>, 
    -	So opposed to having  div> after div> with classes such as  div id”=header/article/footer”> div />, one div id=”page”> can cont ain the header> and nav> elements in its own without sub div>’s. 
    -	The point of creating these new elements is so that the web page authors can use them to help describe the structure of the page. For example, screen reader software might allow users to ignore headers and footers and get straight to the content. Similarly, search engines might place more weight on the content in an article> element than that in the header>, or footer> elements. It also makes the code easier to follow. 
        *	header> and footer> elements can be used for the main header and footer that displays on every page or each individual article or section can have their own header and footer element. 
    -	nav> elements are used to contain the major navigational blocks on the site such as the primary site navigation.
        *	Some Devs use nav> elements for the links that appear at the bottom of a page such as, privacy policy, terms and conditions, and accessibility information. 
    -	article> element acts as a container for any section of a page that could stand alone and potentially be syndicated. 
        *	These can be individual articles, blog post entries, comments, or forum posts. Any independent piece of content. 
        *	If a page contains several articles or such, each would have to live inside its’ own article> element. 
        *	article> can even have other article> elements nested inside of it, in its own child article> elements. i.e. comment sections on a given article or blog post. 
    -	aside> element has two purposes, depending on whether it is inside an article> element or not. 
        *	When inside an article> it should contain information related to the article but not essential to its overall meaning. A pull-quote or glossary for example. 
        *	When outside an article>, it acts as a container for content that is related to the entire page. Such as, links to other sections of the site, a list of recent posts, a search box, or recent tweets/posts by the author. 
    -	section> groups related content together, and typically each section would have its own heading. 
        *	There can be several section> elements	to contain different sections such as, latest news, top products, and newsletter signup.
        *	section> elements can contain related article> elements with common themes and purposes. 
        *	section> should not be used as a wrapper for the entire page. That is still a job for a div>.
    -	hgroup> For grouping headers, h1> through h6>.
    -	figure> and figcaption> - Used to contain any content that is referenced from the main flow of an article. i.e.
        *	Images
        *	Videos
        *	Graphs
        *	Diagrams
        *	Code samples
        *	Text that supports the main body of an article
    -	figcaption> should always accompany a figure> element to provide a text description of the figure> element. 
    -	div> Will remain an important way to group together related elements, because you should not be using these elements for any purpose other than explicitly stated. 
    -	HTML 5 also allows web page authors to place an a> element around a block level element that contains child elements. This allows you to turn an entire block into a link. 

## Process & Design

*   How to approach building a site, understanding your audience and their needs, & how to present information visitors want to see. The following is a process that you can use when you are creating a new website. 
*	Who is the site for?
    -	It can be helpful to ask some questions about the people you would expect to be interested in the subject of your site. 
    -	Clients, when asked, will commonly say “the entire world”. Unlikely!
    -	Even if the subject of your site casts a wide net, your unlikely to be visited by users from other countries, and you can still think about the demographics of a sample of the target audience. 
    -	Target audience individuals:
        *	What is the age range?
        *	Will your site appeal to more women or men? What is the mix?
        *	Users’ country?
        *	Do users live in rural or urban areas?
        *	Average income of users?
        *	Level of education?
        *	Marital or family status?
        *	Occupation?
        *	Hours of work per week?
        *	Web usage?
        *	What kind of device is your target audience likely to be using to access your site?
    -	Target audience companies:
        *	Company size?
        *	Relevant department?
        *	Position of people in the company using your site?
        *	Using for themselves or someone else?
        *	How large is the budget they control? 
    -	You can invent some fictional visitors from your typical target audience. They will become your friends during the design process and can influence design decisions from color palettes to level of detail in descriptions. 
        *	i.e.
            -	Gordon, Male, age 28, from Chicago, teacher making 62k/yr, web usage 2-3 days/wk.
            -	Molly, F, age 47, from San Francisco, attorney making 180k/yr, web usage daily. 
            -	Jasper, M, age 19, from New York, student making 24k/yr, web usage daily. 
                *	If you have questions about the sites’ usage, you can go back and ask yourself, “what would Molly want in this situation”?
*	Why people visit your website?
    -	Your content and design should be influenced by the goals of your users. 
    -	There are two basic categories of questions you can ask to determine why people are coming to your website. 
        *	Key Motivations
            -	Are they looking for general entertainment or do they need to achieve a specific goal?
            -	If there is a specific goal, is it a professional or personal one?
            -	Do they see spending time on this activity as essential or a luxury?
        *	Specific Goals
            -	Do they want general information/research (such as background on a topic/company), or are they after something specific (such as a particular fact or information on a product)?
            -	Are they already familiar with your service/product? Or do they need to be introduced to it?
            -	Are they looking for time sensitive information, such as the latest news/updates on a particular topic?
            -	Do they want to discover information about a specific product or service to help them decide whether to buy it or not?
            -	Do they need to contact you? If so, can they visit in person (which might require opening hours and a map)? Or might they need an email or telephone contact details?
*	What are your visitors trying to achieve?
    -	Looking for key tasks and motivations can help guide your site design.
    -	First create a list of reasons why people would be visiting your site. Then you can assign the list of tasks to the fictional visitors you created earlier in the process.
        *	Gordon loves to play tennis and has had one for several years. Now he has a girlfriend that he is introducing to the sport and wants to buy her one. 
        *	Molly, after reading about your doggy daycare service in the paper, wants to find out if it would be suitable for her. 
        *	Jasper had a bad experience at a hotel and now wants to post a complaint. 
*	What information do your visitors need?
    -	What information do your visitors need in order to achieve their goals quickly and easily?
    -	Look at each reason why people are visiting your site and determine what they need to achieve their goals. 
    -	You can prioritize levels of information from key points down to non-essential or background information. 
    -	By ensuring that you provide the information that your visitors are looking for, they will consider your site more relevant to them. Then you will have an opportunity to tell them any extra information that you think would be helpful to them or expose them to additional products and services you may be promoting. 
        *	Failure to do this means that they will go elsewhere.
    -	Key information:
        *	Will visitors be familiar with your subject area/brand, or do you need to introduce yourself?
        *	Will they be familiar with the product/service/information you are covering, or do they need background information?
        *	What are the most important features of what you are offering?
        *	What is special about what you offer that differentiates you from other sites that offer something similar?
        *	Once people have achieved the goal that sent them to your site, are there common questions people ask about this subject area?
*	How often will people visit your site?
    -	Some sites benefit from being updated more frequently than others. Some information (such as news) may be constantly changing, while other content remains relatively static. 
*	Questions to help decide how often to update your website content…
    -	Goods/services
        *	How often do the same people return to purchase from you?
        *	How often is your stock updated or your service changed?
    -	Information
        *	How often is the subject updated?
        *	What percentage of your visitors would return for regular updates on the subject, compared with those who will just need the information once?

##  Site Maps

*   Now that you know what needs to appear on your site, you can start to organize the information into sections or pages.
*	The aim is to create a diagram of the pages that will be used to structure the site. This is known as a site map, and it will show how those pages can be grouped. 
    -	To help what information should go on each page, you can use a technique called card sorting.
    -	This involves placing each piece of information that a visitor might need to know on a separate piece of paper and then organizing the related information into groups.
    -	Each group relates to a page and, on larger sites, the pages can in turn be grouped together to create different sections of the website.
    -	The groups of information are then turned into the diagram that is known as the site map.
    -	Use your target audience to help you group related information together.
    -	A site map will usually begin with the homepage. Additionally, if the site is large and is compartmentalized into sections, each section might require its own section homepage to link to all of the information within it. 
    -	Most online shops have section homepages for each type of product, which then in turn link to individual product pages. 
    -	Duplicate information may be needed to appear on more than one page. 
    -	The pages (or groups of pages) will inform how users navigate through the site.
    -	Remember to focus on the goals that your visitors want to achieve. 
    -	It is worth noting that the site owner might organize information in a way that is different to what the public expects. It is important to reflect the public’s understanding of the subject (rather than just the site owner’s understanding of it).
        *	Example site map pg. 462

## Wireframes

*   A simple sketch of the key information that needs to go on each page of a site.
    -   Shows the hierarchy of information and how much space it might require.
*	Building wireframes of your site involves sketching or shading areas where each element of the page will go, such as, logo, primary navigation, headings and main bodies of text, user logins, etc. 
*	Don’t include color scheme, font, background, or images in the wireframe. Your focus should be on what information needs to be on each page and create a visual hierarchy to indicate the most important parts of each page. 
*	Showing wireframes to clients is more helpful than showing them a design. This way they can focus on the function instead of how the site looks. 
    -	Example wireframe pg. 464

##  Getting Your Message across using design

*   The primary aim of any kind of visual design is to communicate. Organizing and prioritizing information on a page helps users understand its importance and what order to read it in.
*	Content – web pages often have a lot of information to communicate. 
    -	A masthead or logo
    -	Links to navigate the site
    -	Links to related content and other popular articles
    -	Login or membership options
    -	Ability for users to comment
    -	Copyright information
    -	Links to privacy policies, terms and conditions, advertising information, RSS feeds, subscription options
*	Prioritizing – if everything on a page appeared in the same style, it would be much harder to understand. Key elements would not stand out. 
    -	By making parts of the page look distinct from surrounding content, designers draw attention to (or away from) those items.
    -	Designers create something known as a visual hierarchy to help users focus on the key messages that will draw people’s attention, and then guide them to subsequent messages. 
*	Organizing – grouping together related content into blocks or chunks makes the page look simpler and easier to understand. 
    -	Users should be able to identify the purpose of each block without processing each individual item. 
    -	By presenting certain types of information in a similar/consistent visual style (such as using the same style for all buttons or all links), users will learn to associate that style with a particular type of content. 
*	Visual hierarchy 
    -	Attention is immediately drawn to a picture that shows the service this company offers and a headline to explain it. The size and colored background reinforce that this is the primary message on the page. 
    -	Below in smaller groups would be the details should the service appeal to the user.
*	Grouping 
    -	Chunks of information
        *	Logo and nav is one
        *	Information about company services is another
        *	Broken down details about services and products is a third. 
*	Similarity 
    -	Consistent headings and styles. 
    -	Consistent icons
    -	Consistent colored links 

##  Visual hierarchy

*   Most users do not read entire pages, instead they skim to find information. Use contrast to create a visual hierarchy that gets your key message across and helps users find what they are looking for.
*	Size – larger elements will grab users’ attention first. This is why headings and key points are relatively large.
*	Color – foreground and background color can draw attention to key messages. Brighter sections tend to draw users’ attention first. 
*	Style – an element may be the same size and color as surrounding content but have a different style applied to it to make it stand out. 
    -	These 3 in order create the visual hierarchy. However, there is one element that will often attract the eye first and can say more for your page than an entire page of text. 	
        *	IMAGES

##  Grouping & Similarity

*   When making sense of a design, we tend to organize visual elements into groups. Grouping related pieces of information together can make a design easier to comprehend.
*	Proximity – when several items are placed close together, they are perceived as more related than items placed farther apart.
*	Closure – when faced with a complicated arrangement of items, we will often look for a single or recognizable pattern or form. A real or imaginary box can be formed around elements due to their proximity and alignment. 
*	Continuance – when elements are placed in a line or a curve then they are perceived to be more related than those that are not following the same direction. This can be used to direct the reader from one part of a page to the next. 
*	White space – placing related items closer together and leaving a bigger gap between related items.
*	Color – a background color placed behind related items to emphasize their connection.
*	Borders – a line can be drawn around the border of the group or between it and its neighbors. 
    -	We naturally observe similarities in design, and things that are similar are perceived to be more related than things that are dissimilar. Repetition of similar color, size, orientation, texture, font, or shape, suggest that matching elements have a similar importance or meaning. 
        *	Consistency – makes it possible that having read one block of your page, it is possible to infer the meaning of other related items in that box that follow the same style. 
        *	Headings – giving a chunk of information a heading clearly tells the user whether or not the content of the grouping is relevant to them. If not, they can ignore all of the elements within it. This is also helpful for users with screen readers. 

##  Designing Navigation

*   Site navigation not only helps people find where they want to go, but also helps them udnerstand what your site is about and how it is organized. Good navigation tends to follow these principles.
*	Concise – ideally, the navigation should be quick and easy to read. It is a good idea to limit the number of options in a menu to no more than eight links. These can link to section homepages which in turn link to other pages. 
*	Clear – users should be able to predict the kind of information that they will find on the page before clicking on the link. Where possible, choose single descriptive words for each link rather than phrases.
*	Selective – the primary navigation should only reflect the sections or content of the site. Functions like logins and search, and legal information like terms and conditions and so on are best placed elsewhere on the page. 
*	Context – good navigation provides context. It lets the user know where they are in the website at that moment. Using a different color or some kind of visual marker to indicate the current page is a good way to do this. 
*	Interactive – each link should be big enough to click on and the appearance of the link should change when the user hovers over each item or clicks on it. It should also be visually distinct from other content on the page. 
*	Consistent – the more pages a site contains, the larger the number of navigation items there will be. Although secondary navigation will change from page to page, it is best to keep the primary navigation exactly the same. 
    -	A large site may have primary, secondary, and even tertiary navigation. primary navigation often appears across the top of the site from left to right, or down the left hand side of the page. secondary navigation could be under the primary navigation or down the side of the page. Tertiary navigation often sits  in the footer of the page. The menu will not be the only way users navigate the site. They will also use links within each page. Some sites also offer a search function. 

##  Practical Information

*   Search engine optimization, using analytics to understand visitors, and putting your site on the web.
*	Search Engine Optimization (SEO)
    -	The basics: SEO is the practice of trying to help your site appear nearer the top of search engine results when people look for the topics that your website covers. 
    -	At the heart of SEO is the idea of working out which terms people are likely to enter into a search engine to find your site and then using these terms in the right places on your site to increase the chances that search engines will show a link to your site in their results.
    -	Search engines look at what appears on your site, as well as how many sites link to you and how relevant those links are. For this reason, SEO is often split into two areas:
        *	On-page techniques
            -	Methods you can use on your web page to improve their ratings on search engines. The main component being the keywords people are likely to enter into a search engine to find your site, these keywords then being included in the text and HTML code for your site in order to help the search engine know that your site covers these topics. Search engines rely heavily on text in your pages, for example, ensuring that any images have appropriate text value of their alt”” attributes. 
            -	In every page of your website there are 7 key places where keywords can appear in order to improve findability.
                *	Page title: title> element within the head> that appears in the tab or top of the browser window.
                *	URL/web address: Where possible, use keywords in the file name as this is part of the URL.
                *	Headings: Keywords in the h1> element let a search engine know what a site is all about. 
                *	Text: Repeating keywords in the main body of the text at least 2-3 times helps.
                *	Link Text: Use keywords in the text that create links between pages (as opposed to generic phrases like, “click here”). 
                *	Image alt””: providing accurate description in your image alt attributes helps your images show in image based searches. 
                *	Page Description: Also in the head> element, the meta> element should be a sentence that describes the content of the page. 
    -	Identifying Keywords and Phrases:
        *	Brainstorm: Make a list. Ask yourself and others what words they may use when searching for a particular subject. 
        *	Organize: Group keywords into separate lists for the different sections or categories of your website. 
        *	Research: adwords.google.co.uk/select/keywordtoolexternal, www.wordtracker.com, and www.keyworddiscovery.com, are a few tools available where you can enter your keywords and they will suggest more.
        *	Compare: Look at the competition for your terms. It’s unlikely that your site will appear at the top for every keyword. 
        *	Refine: Now pick which keywords you will focus on. 
        *	Map: Pick 3-5 for each page you have mapped out and incorporate them. 
*	Analytics: Learning about your visitors. 
    -	Using google analytics, you can immediately start analyzing how users are finding your site, what they are looking at, and when they are leaving. The overview page tells you a lot about your visitors. 
*	Domain Names & Hosting:
    -	Domain names: your domain name is your web address. Usually an annual fee, domain name must be available. Lots of domain name sites also offer web hosting. 
    -	Web hosting. Most sites live on web servers run by web hosting companies. When choosing a web hosting company you should consider…
        *	Disk space: total size of all files that make up your site (HTML &CSS).
        *	Bandwidth: Amount of data the hosting company will send to your site’s visitors.
        *	Backups: Check in the company performs backups on your site and how often. Some sites offer access to backups which can be helpful if you make a mistake when updating it. 
        *	Email Accounts: Most host companies will provide email servers. Check the size of mailbox you’re allowed and the number you can use. 
        *	Server-side languages and databases: If you’re using a content management system, it will likely use a server-side programming language and a database (like PHP with MySQL). Be sure your hosting company supports the tech your software needs to run. 
*	FTP & 3rd party tools
    -	File Transfer Protocol allows you to transfer files across the internet from your computer to the web server hosting your site. When purchasing your web hosting, you’ll be given FTP details that you enter into your FTP program in order to connect to the server. Usually this will be an address such as ftp://mydomain.com, a username, and a password. It is important to keep this information secure to prevent strangers from gaining access to your server. 
        *	FTP applications:
            -	FileZilla
            -	FireFTP
            -	CuteFTP
            -	SmartFTP
            -	Transmit
        *	3rd party tools:
            -	Blogs – wordpress, tumblr, posterous
            -	E-commerce – shopify, bigcartel, go.magento
            -	Email newsletters – campaignmonitor, mailchimp
            -	social networking sharing buttons – addthis, addtoany
