# Static Portfolio

## Setup

```bash
# Clone the repository
git clone https://github.com/$USER/yokochi-design.git
# Install static site generator
brew install zola
```

[Brew not found?](https://brew.sh)

## Writing an Post

1. Open `$REPOSITORY/content` directory in Obsidian
2. Create folder - the name will be it's URL path
3. Create `index.md` file in that folder
4. Write frontmatter with following fields (use two spaces to indent):

```yaml
---
title: Article Title
description: Description of the article
date: 2024-01-01
extra:
  role: Role
  timeline: November 2023 - April 2024
---
```
5. Place `thumbnail.webp` in the created directory
6. Start the server from terminal:
```bash
# Change the directory to where the repository is cloned
cd $REPOSITORY
# Start the server
zola serve
# Open the webpage in safari
open http://localhost:1111
```
7. The website should load, and article sould be visible in the list
8. Since obsidian has autosave, the website should live-reload when changes are made