## Commits
- Follow the [Conventional Commits](https://www.conventionalcommits.org) specification.
	- Unscoped `feat` commits are inferred to have `content` scope
		- `feat: update glossary` is the same as `feat(content): update glossary`
		- Explicitly include the `content` scope if needed when a commit has multiple scopes
			- `feat(content, obsidian): ...` implies a change in content as well as Obsidian
	- Changes that meaningfully affect Obsidian should be given the `obsidian` scope 
		- `feat(obsidian): update theme`
		- Meaningful changes to Obsidian should use the `feat` type