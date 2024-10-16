# HTML - HyperText Markup Language

HTML - HTML stands for **Hypertext Markup Language**. It's the standard markup language for creating web pages and web applications. HTML provides the structure and content of a webpage by using a system of tags and attributes.

These tags define the various elements of a webpage such as headings, paragraphs, links, images, forms, and more. Web browsers interpret HTML documents and render them into visual web pages for users to view and interact with on the internet.

## What is Tag, Attributes, Elements, and content?

1.  Tag : Imagine tags like little instruction manuals for the web browser. They come in pairs, a start tag < and an end tag > with the element name in between. For example,
    < h1> is a start tag for a heading element, and </ h1> is its closing tag.

        Ex - img tag for image, p tag for paragraph, h1 to h6 for heading.

2.  Attributes : Attributes provide additional information about HTML elements and are always specified in the opening tag of an element. Attributes are made up of a name and a value, separated by an equal sign (=) and enclosed in double or single quotes. Attributes modify the behavior or appearance of an element.

    Ex : the href attribute in an < a> tag specifies the URL of the link, and the src attribute in an < img> tag specifies the source (URL) of an image.

3.  Content : This is the information that goes between the start and end tags of an element. It can be text, images, videos, or even other HTML elements (elements can be nested within each other). The content determines what the user sees or interacts with on the webpage.

    Ex : 
    ```
    <p>This is Paragraph Content</p>
    ```

4.  Elements : An element is a complete set of tags and their content, including the opening tag, closing tag, and any content nested within them. Together, they define a particular component or piece of content on a webpage.

    Ex : 
    ```
    <p>This is a Paragraph.</p>
    ```

## heading In HTML - Six heading tag

# h1 - Heading 1
## h2 - Heading 2
### h3 - Heading 3
#### h4 - Heading 4
##### h5 - Heading 5
###### h6 - Heading 6

# Q 1. Difference b/w b tage and strong tag, i tag and em tag?

# Fonts tag in HTML

1. **b tag:** The < b> tag is used to make text bold. However, it doesn't carry any semantic meaning and is purely presentational.
2. **strong tag:** Similar to < b>, the < strong> tag also makes text bold, but it carries semantic weight, indicating that the enclosed text is of strong importance.
3. **i tag:** The < i> tag is used to italicize text. Like < b>, it doesn't carry any semantic meaning and is purely presentational.
4. **em tag:** Similar to < i>, the < em> tag italicizes text, but it carries semantic weight, indicating emphasis.
5. **u tag:** The < u> tag underlines text.
6. **s tag:** The < s> tag is used for strikethrough text, indicating that the content is no longer accurate or relevant.
7. **del tag:** Similar to < s>, the < del> tag also represents strikethrough text, but it carries semantic weight, indicating deleted text.
8. **mark tag:** The < mark> tag highlights text with a background color, typically yellow.
9. **sup:** The < sup> tag is used for superscript text, often used for mathematical expressions.
10. **sub:** The < sub> tag is used for subscript text, typically used for footnotes or chemical formulas.

# Type of Tag in HTML

**1. Semantic tag:** A semantic element clearly describes its meaning to both the browser and the developer.

-   Ex - < form> < table> < header> < footer> < article>

**2. Non-semantic tag:** < div> and < span> is non-semantic tag

**3. Self-Closing Tags:** These tags are written with a forward slash (/) directly following the element name and before the closing angle bracket (>). They represent elements that don't contain any content within them.

**Note:** While self-closing tags are valid in HTML, some stricter environments like XML might require them to be closed with separate tags (e.g., < br> instead of < br />).

-   Ex: < br/> (line break), < hr/> (horizontal rule), < img src="image.jpg" alt="Image description" /> (image), < input type="text" name="username" /> (form input field).

**4. Separate Closing Tags:** These involve an opening tag with the element name followed by a closing angle bracket (>), and a separate closing tag that starts with a forward slash (/) followed by the element name and a closing angle bracket (>). They represent elements that can contain content within them.

-   Ex: < p>This is a paragraph.< /p>, < b>Bold text< b/>
    < div>This is a section with content.< /div>

# Type of Element in HTML

**1. Block-Level Element:** Block-level elements typically start on a new line and occupy the full width available (by default). They force a line break before and after their content.

-   Ex: < header>, < nav>, < section>, < article>, < aside>, < main>, < footer>, < h1> to < h6> headings, < p>, < div>, < ul>, < ol>, < table>, < form>, < pre>, and < hr>

**2. Inline Element:** Inline elements typically display their content on the same line with surrounding text and only occupy the space needed for their content. They don't inherently create line breaks.

-   Ex: < span>, < b>, < i>, < strong>, < em>, < a>, < img>, < code>, < em>, < sup>, < sub>, < br>, and most emphasis and formatting tags.

| Feature     | Block-Level Elements                          | Inline Elements                                       |
| ----------- | --------------------------------------------- | ----------------------------------------------------- |
| Line Breaks | Force line breaks before and after by default | Don't inherently create line breaks                   |
| Width       | Occupy full available width (by default)      | Only occupy space needed for their content            |
| Stacking    | Can stack vertically on top of each other     | Can flow horizontally alongside other inline elements |

In HTML, there's a distinction between how tags are used depending on whether they represent elements that can contain content or not. Here's a breakdown of self-closing tags and separate closing tags:

# 1. List in HTML

-   **Definition :** In HTML, a list is a way to organize and display related pieces of content in a structured format. Lists are useful for presenting information in a clear and organized manner, making it easier for users to understand the relationships between different items.

## _Type of HTML List_

**1. Ordered List** An ordered list is defined using the < ol> tag in HTML. Each item within the list is defined using the < li> tag. By default, ordered lists display numbers (1, 2, 3...) to indicate the order of the items.

-   Tag: ol tag (ordered list), li tag (list item)
-   Attributes:
    -   type: This attribute specifies the numbering or lettering style used for the list items. Here are the common options:
        -   type="1" (default): Numbers the list items (1, 2, 3...)
        -   type="a": Lowercase alphabetical lettering (a, b, c...)
        -   type="A": Uppercase alphabetical lettering (A, B, C...)
        -   type="i": Lowercase Roman numerals (i, ii, iii...)
        -   type="I": Uppercase Roman numerals (I, II, III...)
    -   start: This attribute allows you to define a starting number or letter for the list. For example, start="4" would begin the list with "4" instead of "1".
    -   reversed: This attribute reverses the order of the numbering or lettering in the list.

**2. Unordered List:** An unordered list in HTML is used to represent a collection of items where the order doesn't necessarily matter. These lists are typically displayed with bullet points to visually group the items.

-   An unordered list is defined using the < ul> tag in HTML.
-   Each item within the list is defined using the < li> tag.
-   By default, unordered lists display bullet points (●, ◦, etc.) for each list item.
-   Tag: ul tag (unordered list),
-   Attribute:
    -   type="disc" (default): The standard disc bullet (●)
    -   type="circle": A circle bullet (○)
    -   type="square": A square bullet (■)
    -   type="none":  ()

**3. Definition List:** Definition lists in HTML provide a structured way to define terms and their corresponding meanings. They are essentially like mini-glossaries embedded within your web page.

-   Tag:
    -   < dl>: This tag marks the beginning of the definition list.
    -   < dt>: This tag defines the term being explained.
    -   < dd>: This tag defines the description or definition of the term.
-   Attribute:
    -   Definition lists are simple and don't have any specific attributes associated with their tags.
    -   The structure relies on the proper nesting of tags:
    -   The < dl> tag acts as a container for the entire definition list.
    -   Within < dl>, each term being defined is wrapped in a < dt> tag.
    -   The corresponding definition or description for the term goes inside a < dd> tag, always following the < dt> tag for the corresponding term.

# 2. Image and Multimedia

**1. Image:** Used to embed images into a web page.
-   tag: < img /> tag
-   Attributes:
    -   src: (Required) Specifies the path to the image file.
    -   alt: (Highly recommended) Provides alternative text for the image, essential for accessibility and SEO.
    -   width: Sets the width of the image in pixels.
    -   height: Sets the height of the image in pixels.

**2. Video:** Used to embed videos into a web page.
-   tag: video tag (Parent tag), source tag
-   Attributes:
    -   src: (Required) Specifies the path to the video file.
    -   controls: Adds playback controls (play, pause, volume, etc.).
    -   autoplay: Starts playback automatically (use with caution for accessibility).
    -   loop: Plays the video in a loop.
    -   muted: Mutes the video by default.
    -   type: Specifies the MIME type of the video file (optional, browser usually infers).
    -   poster: Sets an image to display before the video plays.
    -   width: Sets the width of the video player in pixels.
    -   height: Sets the height of the video player in pixels.

**3. iframe:** Used to embed content from another website (like a YouTube video) directly into your web page.
-   tag: iframe
-   attributes:
    -   src: (Required) Specifies the URL of the content to embed.
    -   frameborder: Controls the display of a border around the iframe (0 for no border).
    -   scrolling: Controls whether scrollbars appear in the iframe (e.g., "auto", "yes", or "no").
    -   allowfullscreen: Enables fullscreen mode for the embedded content (if applicable).
    -   width: Sets the width of the iframe in pixels.
    -   height: Sets the height of the iframe in pixels.
        **4. Audio:** Used to embed audio files into a web page.
-   tag: audio tag < audio> & source tag < source/>.
-   Attributes:
    -   src: (Required) Specifies the path to the audio file.
    -   controls: Adds playback controls (play, pause, volume, etc.).
    -   autoplay: Starts playback automatically (use with caution for accessibility).
    -   loop: Plays the audio in a loop.
    -   muted: Mutes the audio by default.
    -   type: Specifies the MIME type of the audio file (optional, browser usually infers).
