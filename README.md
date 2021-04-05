# The Chicken Project 

The Chicken Project is a Hugo project that generates the code for [chickenproject.org](https://chickenproject.org/). The website is deployed with Netlify. 

## Prerequisites
Before you can work on the project, you'll need this software on your computer:
(Note: these instructions assume you're using a Mac)

- [homebrew](https://brew.sh/) 
- [git](https://formulae.brew.sh/formula/git)
- [go](https://formulae.brew.sh/formula/go) 
- [hugo](https://formulae.brew.sh/formula/hugo)
- a code text editor like [Atom](https://atom.io/) or [VS Code](https://code.visualstudio.com/)

You'll also need your own accounts for these services: 
- [github](https://github.com/)
- [netlify](https://www.netlify.com/)
- [imagekit](https://imagekit.io/)

## Setup 
To get the codebase on your computer, run these commands from your terminal: 

- `git clone --recursive https://github.com/kimschles/chicken-project-prototype`
- `cd chicken-project-prototype` 

## Working on the Website 
### Making changes to existing pages
To run a server on your computer so you can see changes you make, run this command: 
- `hugo serve -D` 
... then go to the address `localhost:1313` in your web browser. When you make changes to an existing page, they'll show up in the browser. 

### Adding a new blogpost 
If you want to add a new blog post, run this command (change `your-blog-post.md` to the name of the blogpost): 
- `hugo new content/article/your-blog-post.md` 
- Add your writing and pictures 
- When you're ready to publish the post, change draft to false, like this: 
    - `draft: false`

### Making structural changes to the website   
This part is harder, but if you want to make changes to the website (like adding a new section to the navigation), you'll want to look at the [Anake Theme Demo](https://gohugo-ananke-theme-demo.netlify.app/) website, and then try to reverse engineer what's you want to recreate with the [Anake Example Site code](https://github.com/theNewDynamic/gohugo-theme-ananke/tree/master/exampleSite). A good place to start is with the [config.toml](./config.toml) file. 







