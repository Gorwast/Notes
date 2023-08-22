This Markdown cheat sheet provides a quick overview of all  
the Markdown syntax elements.

## Basic Syntax

These are the elements outlined in John Gruber’s original design document. All Markdown applications support these elements.

| Element         | Markdown Syntax                                  |
| --------------- | ------------------------------------------------ |
| Heading         | `# H1 ## H2 ### H3`                              |
| Bold            | `**bold text**`                                  |
| Italic          | `*italicized text*`                              |
| Blockquote      | `> blockquote`                                   |
| Ordered List    | ```1. First item 2. Second item 3. Third item``` |
| Unordered List  | `- First item - Second item<br> - Third item`    |
| Code            | `` `code` ``                                     |
| Horizontal Rule | `---`                                            |
| Links           | `[title](https://www.example.com)`               |
| Image           | `![alt text](image.jpg)`                         |

## Extended Syntax

These elements extend the basic syntax by adding additional features.  
Not all Markdown applications support these elements.

### **Strikethrough**

To strikethrough words, use two tilde symbols (~~) before and after the words.

~~The world is flat.~~ We now know that the world is round.

### **Definition List**

To create a definition list, type the term on the first line.  
On the next line, type a colon followed by a space and the definition.

First Term  
: This is the definition of the first term.

### **Task List**

- [x] Write the press release  
- [ ] Update the website  
- [ ] Contact the media

### **Table**

\| Syntax      \| Description \|  
\| ----------- \| ----------- \|  
\| Header      \| Title       \|  
\| Paragraph   \| Text        \|  

### **Footnote**

To create a footnote reference, add a caret and an identifier inside  
brackets ([^1]). Identifiers can be numbers or words, but they can’t  
contain spaces or tabs. Identifiers only correlate the footnote  
reference with the footnote itself — in the output, footnotes are numbered sequentially.

Here's a sentence with a footnote. [^1]  
[^1]: This is the footnote.

### **Heading ID**

\### My Great Heading {#custom-id}

### **Fenced Code Blocks**

Depending on your Markdown processor or editor, you’ll use three backticks (```) or three tildes (~~~) on the lines before and after the code block.  
You can make the highlighting be specific to a programming language by putting the name of the language after the first three backticks

```json
{
    "firstName": "John",
    "lastName": "Smith",
    "age": 25
}
```

You can see a list of aliases for the highlighting of [supported languages](\fenced_code_blocks_languages.md) here

### **Emoji**

There are two ways to add emoji to Markdown files: copy and paste the emoji into your Markdown-formatted text, or type emoji shortcodes.

You can see the list of [__emoji shortcodes__](OTHER\emoji.md) here.

### **Automatic URL Linking**

Many Markdown processors automatically turn URLs into links. That means if you type <http://www.example.com>, your Markdown processor will  automatically turn it into a link even though you haven’t used brackets.

### **Disabling Automatic URL Linking**

If you don’t want a URL to be automatically linked, you can remove the link by denoting the URL as code with backticks.

`http://www.example.com`
