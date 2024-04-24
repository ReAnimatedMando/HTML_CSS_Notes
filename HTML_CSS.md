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
