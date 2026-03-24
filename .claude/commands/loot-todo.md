Create a todo item in the contributor's LootChest and link relevant context from the current session.

## Instructions

1. Identify the contributor name from $ARGUMENTS. If not provided, ask for it. The contributor's vault lives at `LootChest/<NAME>/`.

2. If `LootChest/<NAME>/` doesn't exist, create the directory and a fresh `Todos.md` file.

3. Read the existing `LootChest/<NAME>/Todos.md` to understand the current format and items.

4. Ask the contributor (if not already clear from context) what the todo is about. Then:
   - Add the todo as a checkbox item (`- [ ] ...`)
   - Under it, add indented sub-items with relevant context gathered from the current session:
     - Links to files involved (relative paths as inline code)
     - Key decisions or findings from the conversation
     - Any research results, tool recommendations, or blockers discovered
     - References to related brain notes if they exist in the vault
   - Use Obsidian-compatible markdown (wikilinks `[[Note Name]]` for internal links)

5. Format example:
```markdown
- [ ] Short description of the task
	- Context: what was discovered and why this matters
	- Related: `path/to/relevant/file.cpp`
	- See also: [[Related Brain Note]]
	- Blockers or open questions if any
```

6. Show the contributor what was added and confirm.
