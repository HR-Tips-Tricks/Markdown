Measly Underline <hr border-top: 1px solid #8c8b8b /> 



# Markdown
Some examples on how to format in Markdown (.md) [README.md]

| Format            | Syntax                                                      | Example |
| ------            |-----                                                        |-----    |
| Headers 	        | \#, \##, \###, \####, \#####, \###### (from h1 to h6)                                                                                                         <br> \<h1>, \<h2>, \<h3>, \<h4>, \<h5>, \<h6>                     |  <h3>This is a h3 header</h3>	|
| Italic  	        | \*Italic Stallion\*  OR \_Italic Stallion\_	                 | *Italic Stallion* 	|
| Bold  	          | \*\*Only the Boldest\*\* 	OR \_\_Only the Boldest\_\_        | **Only the Boldest** 	|
| Bold with nested Italic | \*\*Only \*Italic\* is the Boldest\*\*                | **Only *Italic* is the Boldest**  |
| Italic with nested Bold | \*Italic Stallion is the \*\*Boldest\*\*\*            | *Italic Stallion is the **Boldest***   |
| Both Italic and Bold | \*\*\* Boldest Italic Stallion\*\*\*                     | ***Boldest Italic Stallion***   |
| Strike through 	  | \~\~Strike through text, neat\~\~ 	                         | ~~Strike through text, neat~~ 	|
| Unordered Lists 	| \- Item 1  <br>   \+ Item 2  <br>  \* Item 7777              | <ul><li>Item 1</li><li>Item 2</li><li>Item 7777</li></ol>	  |
| Ordered Lists 	  | 1. Item A  <br>  2. Item 58008	                              | <ol><li>Item A</li><li>Item 58008</li></ol>  	|
| Mixed Lists 	    | 1. Item 6969  <br>   \- item 1a 	                            | <ol><li>Item 6969</li></ol><ul><li>item 1a</li></ul> 		|
| Emojis:exclamation:  | `:+1:  :metal:  :octocat:  :trollface:  :cat2:`            | :+1: :metal: :octocat:  :trollface: :cat2: |
| Line breaks 	    | Some text [Double space + enter] 	Moar Text                  | Some text  <br>  Moar Text 	|
| Block quote 	    | \> Woah, look how cool this is	 <br> \> And on multiple lines! | <blockquote>Woah, look how cool this is <br> And on multiple lines!</blockquote> 	|
| Inline links 	    | \[Description text\](url here) <br> example on right: `github [training wheels](https://try.github.io/)`  	| github [training wheels](https://try.github.io/) 	|
| Check boxes       | \- \[ \] Get service deployed <br> \- \[x\] Have fun while doing it | <img src='/images/chkboxex.png' width='200px' /> |
| Code 	            | \`That sweet code you wanna show;\` 	                       | `That sweet code you wanna show;` 	|
| Code block/ Syntax highlighting 	| \`\`\`A whole bunch of code\`\`\` 	        |  ```HTML A whole bunch of code``` 	|
| Reference Headers | \[Footer Example\](\#heres-a-footer-example)               | [Footer Example](#heres-a-footer-example) |
| Thin Thematic Break  | Measly Underline <br> \-\-\-                                | Measly Underline <hr height:1px>  |
| Thick Thematic Break | Purposeful Underline <br><br> \-\-\-                        | Purposeful Underline <hr> |
| Images 	          | \Text ![Caption\](url to img)<br>example on right: `Nyancat! ![image](/images/nyancat.png)`  | Nyancat! <img src='images/nyancat.png' width='100px' /> 	|
| Link+images 	    | \[\![Caption\](url to img)\](url to a page)\]<br>example of right: `Click me [![me](/images/nyancat.png)](https://www.youtube.com/watch?v=QH2-TGUlwu4)`        | Click me <a href='https://www.youtube.com/watch?v=QH2-TGUlwu4' target="_blank"><img src='images/nyancat.png' width='100px' /></a> |
| Preformatted 	    | \ \ Begin each line with,two spaces or more to,make text look,e x a c t l y,like,you,type i,t. 	|   Begin each line with,two spaces or more to,make text look,e x a c t l y,like,you,type i,t. 	|
| Tables 	          | \| \| Tables \|    Are    \| Coolness \|<br> \|---\|----------\|:-------------:\|------:\| <br> \|alignment\|left\|center\|right\| | (See Below)  |

| | Tables   |      Are      |  Coolness |
|---|----------|:-------------:|------:|
|alignment| left| center | right |


--------


<h3>If you don't like the markup ways, you can actually just code in HTML, like much of this table was done in.</h3>  
  <h2>Here's a footer example</h2>
  The footer subscript <sup color:red;><a>1</a></sup> below is written in HTML.<br>
  You're really bringing me down<sup><a href="\#fn1" id="ref1">1</a></sup>
  
  _Notice_ the ID within the footer subscript's tag: `<sup><a href="\#fn1" id="ref1">1</a></sup>`
  
  We can reference this ID when creating the footer, along with some cool HTML syntax coloring <br>
  
  ```  
    ```HTML   
      text of stuff
    ```
  ```
  
  ```HTML 
      <sup id="fn1">Why are you down here?<a href="#ref1" title="Jump back to footnote 1 in the text.">  ↩  <sub>jump back up there</sub></a></sup>
  ```
  
  Or even some fancy Javascript 
  ```
    Markdown file edit example text: 
    ```Javascript   
      app.use('/image-carousel', proxy(config.proxies.images));
      app.use('/api/images', proxy(config.proxies.images, {
        ProxyReqPathResolver: (req) => {
          const parts = req.url.split('?');
          const queryString = parts[1];
          return `/api/images${queryString ? `?${queryString}` : ''}`;
        },
      }));
    ```
  ```
  Turns into this F.A.F. code
  ```Javascript   
      app.use('/image-carousel', proxy(config.proxies.images));
      app.use('/api/images', proxy(config.proxies.images, {
        ProxyReqPathResolver: (req) => {
          const parts = req.url.split('?');
          const queryString = parts[1];
          return `/api/images${queryString ? `?${queryString}` : ''}`;
      },
      }));
   ```
   
  Cool, right? Let's get nerdy.
  
  
  Note:
    - When mixing HTML and Markdown code, you'll need to do TWO hard Enters after the line before switching to one or the other. 
    - Best practice is just to stick to one language throughout the document.
    
  <br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
  <br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
  
  
<sup id="fn1">Why are you down here?<a href="#ref1" title="Jump back to footnote 1 in the text.">  ↩  <sub>jump back up there</sub></a></sup>
