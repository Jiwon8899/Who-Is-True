# Who Is True?

> A branching Korean narrative game about testimony, media framing, trust, and uncertain truth

## Play

**[Play in your browser](https://jiwon8899.github.io/Who-Is-True/)**

The game is a self-contained Twine export. No installation is required.

## Project summary

`Who Is True?` places the player behind a small bar where conversations with people connected to a public scandal gradually unlock different viewpoints and endings. The player's wording changes which testimony is trusted, how later chapters open, and how the final interpretation is formed.

| Item | Detail |
|---|---|
| Tool | Twine / Harlowe 3.3.9 |
| Language | Korean |
| Structure | 131 passages |
| Chapters | Prologue plus Chapters 1–5 |
| Interaction | dialogue choices, chapter unlock flags, accumulated ending state |
| Build | Single self-contained HTML file |

## Credits and my role

The in-game credits identify **최지원 & 김서영** as co-creators and co-planners. My contribution is presented as a collaborative share rather than sole authorship.

- Co-planned the central mystery and chapter sequence
- Designed dialogue choices around trust, doubt, and media interpretation
- Built and connected branching passages in Twine
- Managed chapter-unlock and ending-state variables
- Replayed alternative routes to check progression and return-to-menu flow

## Design highlights

- The bar works as a stable setting where witnesses with different incentives can be compared.
- Chapters unlock progressively instead of exposing the full story tree immediately.
- Similar dialogue can lead to different downstream states depending on earlier trust choices.
- The final chapter resolves accumulated state rather than relying on one last binary prompt.
- Delayed dissolve transitions establish a slower, conversational rhythm.

See [STORY_DESIGN.md](STORY_DESIGN.md) for a closer look at the structure.

## Scope disclosure

This is a **narrative/game-design work**, not a primary game-programming sample. The exported story contains no project-specific JavaScript or CSS. The implementation evidence is the 131-passage Harlowe structure, variables, links, conditional chapter unlocks, and ending branches embedded in [index.html](index.html).

## Rights

This portfolio release is not open source. Story text and project materials remain copyrighted by their respective creators. See [RIGHTS.md](RIGHTS.md).
