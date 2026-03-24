Onboard a contributor by detecting their git identity and letting them define their personal commit heading style.

## Instructions

1. Get the contributor's local git username:
   ```
   git config user.name
   ```

2. Greet the contributor by name. Explain that this project lets each contributor choose their own commit message heading style.

3. Show examples of existing styles from the project history:
   - **eme** uses leet-speak/creative encoding: `Add L00tCh3st`, `Add R0AdMa9.µ∂`
   - **pjasicek** uses standard descriptive: `Fix Windows compilation`, `Implement level 13 - Chameleon and bossfight is missing`
   - **Denis Papec** uses past tense: `Added comments`, `Fixes for siren projectile`

4. Ask the contributor to describe or demonstrate their preferred commit heading style. They can:
   - Pick an existing style from above
   - Show 2-3 example headings in their own style
   - Describe the rules (e.g., "all lowercase", "emoji prefixes", "conventional commits", etc.)

5. Once the contributor confirms their style, save it to `LootChest/<NAME>/Commit Style.md` where `<NAME>` is their git username uppercased. Create the LootChest folder if it doesn't exist.

   Format:
   ```markdown
   # Commit Style

   ## Convention
   <Description of their chosen style>

   ## Examples
   - `<example 1>`
   - `<example 2>`
   - `<example 3>`
   ```

6. Confirm the setup is complete. Remind them that when they ask Claude to commit, it will follow their personal style by reading their Commit Style note from their LootChest.
