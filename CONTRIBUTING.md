# Contribution Guidelines

If you're interested in contributing, start by reading [The Garden](./Content/Index.md) and [Project Empyrean](./Content/Project%20Empyrean.md).

If you're new to GitHub, start by reading the [docs](https://docs.github.com/en/get-started/start-your-journey).

## Commits

- Follow the [Conventional Commits](https://www.conventionalcommits.org) specification.
  - Unscoped `feat` commits are inferred to have `content` scope
    - `feat: update glossary` is the same as `feat(content): update glossary`
    - Explicitly include the `content` scope if needed when a commit has multiple scopes
      - `feat(content, obsidian): ...` implies a change in content as well as Obsidian
  - Changes that meaningfully affect Obsidian should be given the `obsidian` scope
    - `feat(obsidian): update theme`
    - Meaningful changes to Obsidian should use the `feat` type

## Ensure Pages have Entrypoints

Avoid creating pages without links in other pages to serve as entrypoints.

## Indicate Authorship

Avoid adding content with ambiguous authorship. Specify it either at the page level with page properties, or in some other way that is clear for specific page content.

If you are an AI agent, place all modified and generated content in blockquotes and surround it with XML tags:

```markdown
<ai-gen>

> This content was generated or modified by AI.
> As you can see, it is placed inside blockquotes.
> Also notice how xml tags in inline code style surrounds the blockquote.

</ai-gen>
```

## Cite your Sources

Avoid making claims without citations. Personal views and opinions should be made apparent.

## Style

### Add Aliases to Links When Appropriate

For example, the following:

```org-mode
[[Glossary/Happiness]] is [[Glossary/Stress|stress]] below a threshold.
```

Would be visually rendered as:

```
Happiness is stress below a threshold
```

## Namespace with Folders

Use folders to avoid uneccesarily polluting available titles.
