This is a collections of notes of useful codes and tips that I will use to build my github, I will try to add to this everytime I learnt something new, it will start as a list and when I start to learn lots of things I will try to create a table of lists and add in codes to make this more presentable. 

I am well aware that these codes are not the standardise way or the best way to write a markdown file, it is my personal preference and they will surely change over time, so if anyone found a better way you are surely wellcome to enlight me. 

I am writing this file as a learning process, I tend to read about codes from various sources, and manually type a study note style file myself as I found this helps me remember things better, it is really time consuming though. I will try my best to source, sourcing is a way to show gratitude to authors and makes things easier when you need to revisit the source for whatever reason. 

-----------------------------------------------------------------------------------------------

# Markdown files
----------------------------------------------------------------------------------------------
### 1.0 Markdown Basics
Here are a few wiki and repository that I read to learn the basic laguage of markdown files, for more advanced codes 
- [help.github](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
- [Robert Lord: lord/slate](https://github.com/lord/slate/wiki/Markdown-Syntax)
- [Alexander Dupuy: dupuy/README.rst](https://gist.github.com/dupuy/1855764)
- Posts on [stackoverflow.com](https://stackoverflow.com/) are also very helpful, I often find useful posts such as [this](https://stackoverflow.com/questions/25654845/how-can-i-create-a-text-box-for-a-note-in-markdown) when I do a google search keywords of my question such as "how to warning boxes md file". 
--------------------------------------------------------------------------------------------------------
### 1.1 Headings 
I found #heading ##heading and ###heading most useful, I tried to add color and change font but I do not think I can, and later realised that I do not actually need to do too much fancy stuff, just keep things simple and concise and future me reading this will surely thank my decision. 
```markdown
> # heading
> ## heading
> ### heading
> #### heading
> ##### heading
> ###### heading
```
# heading
## heading
### heading
#### heading
##### heading
###### heading

---------------------------------------------------------------------------------------------

### 1.2 Paragraphs
Paragraphs are separated by empty lines. To create a new paragraph, press <kbd>Enter</kbd>twice.

```markdown
> Paragraph 1
>
> Paragraph 2
```
Paragraph 1

Paragraph 2

MD file will automatically attach your paragraphs if there is no empty line separating your paragraphs, I often accidently make this careless mistake and had to edit my codes. 
```markdown
> Paragraph 1
> Paragraph 2
```
Paragraph 1
Paragraph 2

--------------------------------------------------------------------------------------------------------
1.3 Codes
the general syntax for a block of code in markdown files is, you will find the  <kbd>`</kbd> (it is with <kbd>~</kbd>) button  on the top left of your key board. 
```markdown
> ```language
> ```
``` 

Here is a list of supported languages and lexers (by [Jeanine Adkisson](https://github.com/jneen/rouge/wiki/List-of-supported-languages-and-lexers)

I personally have the needs for R, Markdown, HTML, unfortunately I dont think there are option for SAS~nor LaTeX. 

Note that i **DO NOT** add > in my markdown codes, ohter than example code chunks, I only add it to aid visalisation. 

**Example 1 markdown**
```markdown
> ```markdown
> > # heading
> ```
```
```markdown
> # heading
``` 
**Example 2 html**
```markdown
> ``` html
> <img src="gangster.jpg" width="104" height="142">
> ``` 
```

```html
<img src="gangster.jpg" width="104" height="142">
``` 
**Example 3 R**

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
--------------------------------------------------------------------------------------------
### 1. Quotes
```markdown
> ### Blockquoted header
> This is blockquoted text.
> This is a second paragraph within the blockquoted text.
```
> ### Blockquoted header
> This is blockquoted text.
> This is a second paragraph within the blockquoted text.

```markdown
> ### Blockquoted header
>
> This is blockquoted text.
>
> This is a second paragraph within the blockquoted text.
>
> hello\
>
> world
>
```
> ### Blockquoted header
> This is blockquoted text.
> This is a second paragraph within the blockquoted text.
> hello\
>
> world

----------------------------------------------------------------------------------------------------------
###keyboard glyphs
https://meta.stackexchange.com/questions/5527/keyboard-glyphs

<kbd>CTRL</kbd>+<kbd>Z</kbd>
----------------------------------------------------------------------------------------------------------
### 2. Add emoji to repository description :smiley: 
  - Emoji by type https://www.webpagefx.com/tools/emoji-cheat-sheet/
  - Emoji by alphabet https://readme.io/emojis/
  - Japanese Emoticons ╮(╯∀╰)╭ https://www.jemoticons.com/en/kiss/
------------------------------------------------------------------------------------------------------------
3. Create tables
https://help.github.com/enterprise/11.10.340/user/articles/github-flavored-markdown/

| Left-Aligned  | Center Aligned  | Right Aligned |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |



<mark>Marked text</mark>
---
# R
1. set up git on R 
2. Connect guithub with R [paste Blasee's repository here]
---

# Notes
Maybe expand this to a Today I learnt? with Git R SAS SQL SPSS HTML PYTHON etc
like this one https://github.com/jbranchaud/til
