# Dependencies
1. `npm`, `nodejs`: following [https://nodejs.org/en/download](https://nodejs.org/en/download)
2. `hugo`: can be installed as a python module (pip3 install hugo) OR through package manager (`apt install hugo`)

# Initial set up
1. From hugo_examplesite/themes/dot-org-hugo-theme, run `git pull`
2. From hugo_examplesite/, run `cp themes/dot-org-hugo-theme/exampleSite/package.json .` and `cp themes/dot-org-hugo-theme/exampleSite/postcss.config.js .`
3. From hugo_examplesite/, run `npm install`

# Testing
1. Either `npm start` or `hugo serve`, both works

# Configuration
All configuration files are in `config/_default`. The configuration options are split into 3 files. 
- hugo.yaml:  title, timezone
- languages.yaml: navbar items
- params.yaml: links with icons showed on footer (by default mail, whatsapp weren't supported. Custom icons can be added in `static/img/social-icons/`)

# Adding content
`hugo new content filename.md` (for example, `hugo new content examplepage.md`, will add `content/en/examplepage.md`)
Then simply edit the files in `content/en/`. `content/en/_index.md` file is the home page that people would see.
There are some special syntaxes for adding things like columns, line breaks, etc. that can be found on the theme's documentations.
**make sure to set `drafts: false`** when editing the file

# Adding blogs
`hugo new content blogs/blogname.md` 

# Adding images
All images go to `/static/img`. 

# Docs
The documentation for the theme [https://github.com/cncf/dot-org-hugo-theme](https://github.com/cncf/dot-org-hugo-theme) (Skip Installation, Installing Dependencies sections)
Getting started guide for Hugo: [https://gohugo.io/getting-started/quick-start/](https://gohugo.io/getting-started/quick-start/)
