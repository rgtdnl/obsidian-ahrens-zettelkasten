# Stock Ahrens Zettelkasten Vault

A deliberately minimal Obsidian vault that implements the Zettelkasten method exactly as Sönke Ahrens describes it in *How to Take Smart Notes*. No plugins, no database views, no category system, no frontmatter taxonomy. Six folders, four templates, one index. Obsidian's built-in backlinks and graph view provide everything else.

## Why this vault exists

The book's premise is that the structure must stay simple so the complexity can build up where it belongs: on the content level.

> "The best way to deal with complexity is to keep things as simple as possible and to follow a few basic principles. The simplicity of the structure allows complexity to build up where we want it: on the content level." (p. 20)

Ahrens lists four tools and no more: something to write with, a reference system, the slip-box, an editor. "More is unnecessary, less is impossible." (p. 47)

This vault is that list translated to Obsidian, and nothing else. Where the book says nothing, the vault adds nothing; the next section spells out what that means in practice.

## What is deliberately absent

- **No database views or embeds.** No filtered tables, no live queries rendered inside notes.
- **No frontmatter taxonomy.** No `status`, `rating`, `type`, `topics`, `categories` properties. The only frontmatter is what the method needs: a creation date, and source/author/year on literature notes.
- **No maps of content.** The slip-box has an index, which is in the book; MOCs are a community adaptation and are not included.
- **No plugins required.** Backlinks and the graph view are built into Obsidian.

When to reconsider: if the slip-box grows past roughly 50 permanent notes and finding orphan notes or tracking reading progress becomes a real pain, filtered views are worth adding. They can be introduced at that scale without changing the vault's structure.

## Folder structure

| Folder | Purpose |
|---|---|
| `00 inbox/` | Flat landing zone for fleeting notes, clippings, and raw literature notes. Everything here is processed within 1-2 days, then removed. Goal state: empty. |
| `10 literature/` | Literature notes: source ideas translated into your own words, each with a reference and locator. |
| `20 slip-box/` | Permanent notes: one idea per note, full sentences, written as if for print. Plus `01 index.md`, the entry-point list. |
| `30 projects/` | One subfolder per piece of writing: outlines, drafts, collected notes. |
| `40 archive/` | Finished project folders only. "The bin for the indecisive." |
| `50 templates/` | Four note-type templates. |

Every folder starts with `00 guide.md` describing its purpose, rules, and daily action. Read the guides in order before anything else.

## Note types (from the book)

| Type | Format | Lifecycle |
|---|---|---|
| Fleeting | Reminders, any format, one place | Processed within 1-2 days, then deleted or turned into a permanent note |
| Literature | Ideas in your own words, reference included | Brief is fine: the context is the text. Raw material for permanent notes |
| Permanent | One idea, full sentences, self-contained, linked | Never thrown away. The filename is the claim |
| Project | Outlines, drafts, to-dos for one project | Discarded or archived when the project ends |

## The workflow

1. **Capture** — fleeting notes land flat in `00 inbox`, nowhere else.
2. **Read with a pen** — while reading, write literature notes in your own words with locators; store them in `10 literature`.
3. **Turn to the slip-box** — review the inbox and your literature notes. Write permanent notes: one idea per note, full sentences, in a way your future self can understand without the original context.
4. **File and link** — place each new note behind the note it continues, link both ways, add it to the index if it opens a new thread. Ask: "In which context will I want to stumble upon this again?" — not "Which topic does this belong to?"
5. **Develop ideas** — topics grow bottom-up from the links. Use the index as entry points, follow threads, let contradictions surface.
6. **Write** — when a topic is ready, assemble the relevant permanent notes into a project folder in `30 projects`, arrange them, and turn them into continuous text.
7. **Finish** — move finished project folders to `40 archive`, or delete them. Permanent notes never leave the slip-box.

## Getting started

1. Clone the repo and open the folder as a vault in Obsidian:
   `git clone https://github.com/rgtdnl/obsidian-ahrens-zettelkasten.git`
2. Set the template location: Settings > Templates > Template folder location → `50 templates`.
3. Set the date format to `YYYY-MM-DD` (the templates use `{{date:YYYY-MM-DD}}`).
4. Read the six `00 guide.md` files, starting with `00 inbox`.
5. Start with the `literature` and `permanent` templates; add the others when you need them.
