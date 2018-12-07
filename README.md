This is a collections of notes on useful codes and tips that I will use to build my github, I will try to add to this everytime I learnt something new, it will start as a list and when I start to learn lots of things I will try to create a table of lists and add in codes to make this more presentable. 

I am well aware that these codes are not the standardise way or the best way to write a markdown file, it is my personal preference and they will surely change over time, so if anyone found a better way you are surely wellcome to enlight me. 

I am writing this file as a learning process, I tend to read about codes from various sources, and manually type a study note style file myself as I found this helps me remember things better, it is really time consuming though. I will try my best to source, sourcing is a way to show gratitude to authors and makes things easier when you need to revisit the source for whatever reason. 

-----------------------------------------------------------------------------------------------

# Markdown files
----------------------------------------------------------------------------------------------
### 1.0 Markdown Basics
Here are a few wiki and repository that I read to learn the basic laguage of markdown files
- [help.github](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
- [Bitbucket Markdown syntax guide](https://confluence.atlassian.com/bitbucketserver/markdown-syntax-guide-776639995.html)
- [Robert Lord: lord/slate](https://github.com/lord/slate/wiki/Markdown-Syntax)
- [Alexander Dupuy: dupuy/README.rst](https://gist.github.com/dupuy/1855764)
- Posts on [stackoverflow.com](https://stackoverflow.com/) are also very helpful, I often find useful posts such as [this](https://stackoverflow.com/questions/25654845/how-can-i-create-a-text-box-for-a-note-in-markdown) when I do a google search keywords of my question such as "[warning boxes md file](https://www.google.co.nz/search?q=warning+boxes+md+file&rlz=1C1GGRV_enNZ816NZ816&oq=warning+boxes+md+file&aqs=chrome..69i57.527j0j7&sourceid=chrome&ie=UTF-8)". 
- [R-Studio cheat sheet](https://www.rstudio.com/wp-content/uploads/2015/02/rmarkdown-cheatsheet.pdf)
--------------------------------------------------------------------------------------------------------
### 1.1 Headings 
I found #heading ##heading and ###heading most useful, I tried to add color and change font but I do not think I can, and later realised that I do not actually need to do too much fancy stuff, just keep things simple and concise and future me reading this will surely thank my decision.

You can also use === and --- but I don not recommend it because it makes codes messy, but I can see why some people prefer to use it, I often use these codes in Microsoft Word.

```markdown
> # heading 1
> ## heading 2
> ### heading 3
> #### heading 4
> ##### heading 5
> ###### heading 6
> heading 1
> ===
> heading 2
> ---
```
# heading 1
## heading 2
### heading 3
#### heading 4
##### heading 5
###### heading 6
heading 1
===
heading 2
---
---------------------------------------------------------------------------------------------

### 1.2 Paragraphs
Paragraphs are separated by empty lines. To create a new paragraph, press <kbd>Enter</kbd> <kbd>Enter</kbd>.

```markdown
> Paragraph 1
>
> Paragraph 2
```
Paragraph 1

Paragraph 2

MD file will automatically attach your paragraphs if there is no empty line separating your paragraphs. 

```markdown
> Paragraph 1
> Paragraph 2
```
Paragraph 1
Paragraph 2

--------------------------------------------------------------------------------------------------------

### 1.3 Text

Basic *italic* and **bold** text will be useful, however use of  ``*`` and ``**`` is ineffecient and limiting. You can use shortcuts <kbd>ctrl</kbd> + <kbd>I</kbd>  and <kbd>ctrl</kbd> + <kbd>B</kbd>, however I noticed it works on Unversity PC but not on my Laptop. 

| Style             | Syntax    | Keyboard shortcut             | Code               | Output            |
| :---------------: |:---------:| :----------------------------:|:------------------:| :----------------:|
| Italic            | ``* *``   | <kbd>ctrl</kbd> + <kbd>I</kbd>| ``*Italic*``       | *Italic*          |
| Bold              | ``** **`` | <kbd>xtrl</kbd> + <kbd>B</kbd>| ``**Bold**``       | **Bold**          |
| Strike through    | ``~~ ~~`` |                               | ``Strike through`` | ~~Strike through~~|

Note: To write out astrisks ``*`` without activating it as syntax, use <kbd>``</kbd> to include inline code blocks. 

```markdown
> ``Code``
``` 

``Code``

--------------------------------------------------------------------------------------------------------

### 1.4 Code blocks
the general syntax for a block of code in markdown files is, you will find the  <kbd>`</kbd> (it is with <kbd>~</kbd>) button  on the top left of your key board. 

```markdown
> ```language
> ```
``` 

Here is a list of supported languages and lexers (by [Jeanine Adkisson](https://github.com/jneen/rouge/wiki/List-of-supported-languages-and-lexers))

I personally have the needs for R, Markdown, HTML, unfortunately I dont think there are option for SAS nor LaTeX. 

Note that i **DO NOT** add > in my markdown codes, other than example code chunks, I only add it to aid visalisation. 

**Example 1: Markdown **
```markdown
> ```markdown
> > # heading
> ```
```
```markdown
> # heading
``` 
**Example 2: HTML**
```markdown
> ``` html
> <img src="gangster.jpg" width="104" height="142">
> ``` 
```

```html
<img src="gangster.jpg" width="104" height="142">
``` 
**Example 3: R**
Note that in RMD files, we use {R} rather than R{}. 
```markdown
> ```r {}
> k = vector() # add notes here
> for (i in 1:n){
> k[i] = i^2+5*i
> k
> }
> ``` 
```

```r {}
k = vector() # add notes here
for (i in 1:n){
k[i] = i^2+5*i
k
}
``` 

---------------------------------------------------------------------------------------------

### 1.5   Links

Markdown files will automatically creates links when valid URLs are written. However it is often not presentable, so to reduce the length and use description text you can create an inline link by wrapping link text in brackets [ ], and then wrapping the URL in parentheses ( ). 

You can also use the keyboard shortcut <kbd>ctrl</kbd> + <kbd>k</kbd>to create a link.

```markdown
> https://github.com/JungXue
>
> [Jung Xue](https://github.com/JungXue).
```
https://github.com/JungXue

[Jung Xue](https://github.com/JungXue)

---------------------------------------------------------------------------------------------  

### 1.6 Quotes
I see alot of people used blocked quotes in their md files, so it is definitely very useful.
However for some reason <kbd>Enter</kbd> , <kbd>Enter</kbd> does not work here, so I have to use <kbd>\</kbd> , <kbd>Enter</kbd> here. 
```markdown
> > ### Blockquoted header
> > This is blockquoted text.
> > This is a second paragraph within the blockquoted text.
```
> ### Blockquoted header
> This is the first paragraph.
> This is the second paragraph. 

```markdown
> > ### Blockquoted header
> >
> > This is the first paragraph.
> >
> > This is the second paragraph. 
> >
> > hello\
> >
> > world
> >
```
> ### Blockquoted header
> This is the first paragraph.
> This is the second paragraph. 
> hello\
>
> world

-----------------------------------------------------------------------------------------------
### 1.7 Lists 

```markdown
> 1. Potato
> 2. Tomato
> 3. Tato
```
1. Potato
2. Tomato
3. Tato

```markdown
> - Regression
> - ANOVA
> - MANOVA
```

- Regression
- ANOVA
- MANOVA

Note: <kbd>*</kbd> also forms a list but I avoid it because it may interrupt syntax for bold text <kbd>``*``bold``*``</kbd>.

----------------------------------------------------------------------------------------------------------
### 1.8 keyboard glyphs

You can create keyboard glyphs by using ``<kbd> </kbd>``, this is extremely useful for informing which key to press. 

Some people even made a whole keyboard with kbd, people have eway too much time to spare. See [This](https://meta.stackexchange.com/questions/1939/kbd-elements-are-way-too-intrusive).

```markdown
> <kbd> ctrl</kbd> + <kbd> B </kbd>
```

<kbd> ctrl</kbd> + <kbd> B </kbd>

# continue here

<aside class="notice">
You must replace `meowmeowmeow` with your personal API key. 
</aside>
Use class="notice" for blue notes, class="warning" for red warnings, and class="success" for green notes.


###keyboard glyphs
https://meta.stackexchange.com/questions/5527/keyboard-glyphs

<kbd>CTRL</kbd>+<kbd>Z</kbd>
----------------------------------------------------------------------------------------------------------
### 2. Add emoji to repository description :smiley: 
  - Emoji by [type](https://www.webpagefx.com/tools/emoji-cheat-sheet/)
  - Emoji by [alphabet](https://readme.io/emojis/)
  - Japanese Emoticons ╮(╯∀╰)╭ (by [Tsutomu Narushima](https://www.jemoticons.com/en/))
  - Japanese Emoticons （。ω。 三 ゜ω゜）としろうだよ ([Name diagnosis](https://shindanmaker.com/360578?fbclid=IwAR1gN16jGqWwpBVAYPg33KeN4ZLmXzEzOBZoBEC8jjuIp8L5EdmtfZ7nlpw))
------------------------------------------------------------------------------------------------------------
3. Create tables
https://help.github.com/enterprise/11.10.340/user/articles/github-flavored-markdown/

| Left-Aligned  | Center Aligned  | Right Aligned |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |


Username ``@mentions``
Typing an @ symbol, followed by a username, will notify that person to come and view the comment. This is called an ``“@mention”``, because you’re mentioning the individual. You can also ``@mention`` teams within an organization.

<mark>Marked text</mark>
---
# R
1. set up git on R 
2. Connect guithub with R [paste Blasee's repository here]
---

# Notes
Maybe expand this to a Today I learnt? with Git R SAS SQL SPSS HTML PYTHON etc
like this one https://github.com/jbranchaud/til

# disclaimer
Opinions expressed are solely my own and do not express the views or opinions of my university or employer.
I did not intend to copy or redistribute materials or works of other people, all works are original. 
