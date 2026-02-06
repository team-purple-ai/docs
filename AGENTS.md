# p0 documentation agent instructions

## Product context

- **Product name**: p0 (always lowercase, never "P0" or "p-zero")
- **Company**: Purple / bepurple.ai
- **What it is**: An Electron desktop app for AI-powered coding assistance using Claude

## Terminology

- Use "workspace" not "project"
- Use "session" not "conversation"
- Capitalize "Plan mode" and "Agent mode"
- Use "spec-driven workflow" (lowercase "spec")
- Use "worktree" not "work tree" or "work-tree"
- Use "sub-chat" (hyphenated)

## Mintlify basics

- Configuration lives in `docs.json` — check it before making structural changes
- Use MDX format for documentation pages
- Run `mint dev` locally to preview changes before committing
- Run `mint broken-links` to check for broken links

## Mintlify components

Use Mintlify's built-in components for consistent formatting:
- `<Card>` and `<CardGroup>` for feature grids and navigation
- `<Steps>` for sequential procedures
- `<Tabs>` and `<Tab>` for OS-specific or alternative content
- `<Accordion>` and `<AccordionGroup>` for collapsible sections
- `<Frame>` for images and screenshots
- `<Tip>`, `<Note>`, `<Warning>`, `<Info>` for callouts
- `<CodeGroup>` for multi-language or multi-file code blocks

See https://www.mintlify.com/docs/components for the full component reference.

## Style and formatting

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- When referencing UI elements, use bold: Click **Settings**
- Use code formatting for file names, commands, paths, and code references
- Keyboard shortcuts: use `Cmd` for macOS, `Ctrl` for Windows/Linux

## Screenshot placeholders

Until screenshots are captured, use this format:

```mdx
<Frame>
  <img src="/images/screenshots/descriptive-name.png" alt="Description of what's shown" />
</Frame>

{/* TODO: Screenshot - Detailed capture instructions */}
```

## Content structure

- Add frontmatter (`title`, `description`) to every page
- Use `sidebarTitle` in frontmatter if the nav title should differ from the page title
- Include introductory context before diving into steps or details
- Add "Next steps" or related links at the bottom of pages where helpful

## What to avoid

- Don't edit `docs.json` without understanding the navigation structure
- Don't remove existing pages without checking for inbound links
- Don't use HTML when an MDX component exists for the same purpose
- Don't add pages to navigation that don't exist yet
- Don't refer to p0 as "P0" — it's always lowercase
