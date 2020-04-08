# Wikid

An experiment in building a non-web maintained wiki serving itself over 9p and http read-only. 

Core concepts:

- Pages are a file/directory hierarchy (tree)
- Pages are written in Markdown
- Wikid does not update/edit the tree through the web or 9p
  - Ideally, the tree should be externally version-controlled in a self-pull'ing capacity through cron, etc. 
- Unchanged pages are cached
- Wikid provides a page search walking the cache, then tree
- Wikid provides a page index generated when the tree is updated

## Dependencies



## Build



## Usage



## Structure

```
wiki/		# pages of the wiki (markdown)

templates/	# template files for pages (html and js)

frontend/	# elm source

backend/	# go server source

mkfile		# ‘mk templates’ to generate templates and ‘mk all’ to rebuild backend
```
