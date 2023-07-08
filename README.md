# About this Website

This website is created as a student project for the Northwestern Masters in Data Science 431 - Intro to Go class series.  The purpose was to create an illustrative website using Hugo / Go that demonstrates a fake AI company.

# Assignment Prompt

### Management Problem

The founders of a technology startup saw the market potential of personal knowledge base products. Their pitch to an initial group of investors was straightforward:

*Personal knowledge base products tap into a need we all have: to organize our ideas over time. We read something and make a note of it. We read something else and make another note. We see that things are related and make a note of that as well. At one time or another, everyone has used a Google KeepLinks to an external site. or Microsoft OneNoteLinks to an external site.. Memo-makers and note-keepers opened the door to personal knowledge bases. ObsidianLinks to an external site. walked through that door, moving further along. They see that the power isn't in the individual notes, but in the links between the notes. To foster creativity and productivity, we need a kind of mind-map or graph database of ideas. But Obsidian, as currently defined, has limited potential. What user in the general public knows Markdown, which is needed for formatting the Obsidian notes? And why ask the user to manually enter links between ideas when AI can do it automatically? We can do better than Obsidian, and we have the technical savvy to pull it off.*

The investors seemed intrigued by the initial the product concept, but they were reluctant to fund the startup until they heard that the principals were Go programming experts. The utility of Go for implementing complex technology solutions cannot be denied. (Note the success stories at https://go.dev/Links to an external site..) 

The founders have an initial investor group on-board, but they need additional investors before beginning what will likely be a year-long task of developing the first version of their personal knowledge base product. They decide to use their Go programming skills to build a company website. It can be a static website initially, something to promote the brand name and product idea.

### Assignment Requirements 

Suppose you are a founder of the startup. You need to implement a website using HugoLinks to an external site., the Go static site generator. Methods for doing this are described on the Building WebsitesLinks to an external site. page of the Learning Go for Data Science website. 

* Define a name for your company.
* Pick a Hugo themeLinks to an external site. for the company website (each student should select a unique theme)
* Generate initial pages describing your plans for the personal knowledge base product.
* Using Markdown, Go templating, and git, create and revise the content pages for the website. 
* To get started with Hugo, most gophers pick a Hugo ThemeLinks to an external site. and then add content under the assets/images and content directories. The menu structure for the site is defined under config/_default.
* Complete the Hugo code for the website and run the code locally using hugo serve.
* Upload your local git repository to GitHub.
* Host your website for free on Netlify or GitHub Pages.

# What I Used

This website pulls together a bunch of different pieces:

1. Hugo as the templating engine for the website
2. [Up Business Theme](https://themes.gohugo.io/themes/up-business-theme/) as the theme for the website
3. ChatGPT for most of the lorem ipsum text.  See the website for more details, but I gave ChatGPT a prompt to essentially make as silly / jargony a website as possible
4. StableDiffusion for most of the images.  These were pulled straight from ChatGPT's suggested image prompts
5. My own brains.  Especially on the "real" page and bio page, to demonstrate the power of markdown to create tables, inline links, etc

# What Went Wrong

So this was all for a class project so I had to be pragmatic in getting issues resolved.  If this were a real website, some of the issues identified below would need to be addressed.

* Website is currently using the San Francisco font.  As raised in an issue on the Up Business theme, this font can only be used for UI/UX demonstrations.  So in any real context it would need to change.  Unfortunately, while digging in on how to resolve this I somehow created an unsolvable error that required me to delete my entire project and start from scratch
* I screwed up github versioning for the theme, so as the theme continues to update it would be somewhere between manual updates and impossible to ensure it's reflecting the correct changes

Random bugs I issued that had to be resolved:
* The hero image wouldn't update.  Turns out that the theme template I used hard-coded the reference to an image, overriding any dynamic calls.  I simply redirected the hardcoded reference but this is obviously a bad solution
* Creating new pages on the website would crash the entire thing.  Turns out it was based on how I was creating the front matter / yaml for the pages: I was writing it in Mac textedit and then copy/pasting, which means that rather than having straight braces (") I had curly braces (“”).  D'oh
* I wanted my markdown tables to have stronger column / row breaks but that required edits to the underlying css.  Didn't feel like dealing with that