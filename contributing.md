# Contribution Guidelines

This list records real Pele projects. Pele is the Mermaid-to-SVG renderer at [obsidianmd/pele](https://github.com/obsidianmd/pele). The list itself is not an official Obsidian project.

## What belongs here

- A project whose main purpose is to use, embed, port, or document Pele.
- A public repository or documentation page that you have opened and that matches the description.
- Work in progress, when the repository says so. End that description with `Work in progress.`

Do not add a project that only shares the name Pele, only mentions Pele as one possible downstream renderer, or no longer resolves. Do not describe a third-party project as an Obsidian or kepano project.

## Format

Add the entry at the bottom of the matching category in `README.md`, then add the same entry, with the same URL, to `README.zh-TW.md`.

```markdown
- [Name](https://example.com) - Description that starts with a capital letter and ends with a period.
```

- One entry per line. Do not hard-wrap the description.
- The link text is the project name. Use a scope or qualifier only when two projects share a name.
- Link to the project repository. For a package inside a monorepo, link to that package's directory.
- Official Pele pages stay in **Official**, in reading order. Do not add them to the bottom.
- Keep the table of contents in sync, and do not list Contributing or Footnotes there.
- Check spelling and remove trailing whitespace.
- Search existing entries before adding one.

Descriptions should say what the project does. Leave out slogans, star counts, and version pins that will go stale, except where a port states the Pele version it targets.

## Pull requests

One project per pull request is enough. The title should name the project. In the body, say which category you chose and confirm that the link opens.
