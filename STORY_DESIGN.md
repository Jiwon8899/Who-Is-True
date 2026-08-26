# Story design notes

## Core premise

The player is a bartender listening to people who hold partial and potentially biased views of a public controversy. Because the bartender is not the investigator or the celebrity at the center of the event, the game focuses on interpretation: whom the player encourages, challenges, or dismisses.

## Structural approach

The exported game contains 131 Twine passages. Its main screen progressively reveals Chapters 0–5 using state flags. Individual conversations branch through trust/doubt choices and later converge into chapter-completion passages that update the next unlock or ending state.

```text
Main menu
  └─ Chapter 0: premise and first uncertainty
      └─ Chapter 1: a third party's account
          └─ Chapter 2: media framing
              └─ Chapter 3: competing interpretations
                  └─ Chapter 4: an older connection
                      └─ Chapter 5: accumulated ending state
```

This diagram describes the chapter spine. The actual passage graph branches repeatedly inside each chapter.

## Choice design

- **Trust:** support a speaker and allow their interpretation to shape later state.
- **Doubt:** challenge assumptions or refuse to endorse an incomplete account.
- **Distance:** avoid taking a position, which can preserve uncertainty but close other routes.
- **Help:** move from interpretation toward intervention when the player believes action is justified.

The choices are written as spoken dialogue, so the player chooses both a position and a social tone.

## State design

Harlowe variables track:

- which chapters are available;
- which speaker/route endings have been reached;
- accumulated ending state;
- return paths to the chapter menu.

The result is closer to an interactive screenplay than a free-roaming game. That is why this repository is categorized as a supporting narrative-design project.

## QA focus

- Every visible choice should lead to an existing passage.
- Completing a chapter should unlock the intended next chapter.
- Returning to the main screen should preserve current story flags.
- Alternative trust/doubt routes should not overwrite unrelated branch state.
- Credit and main-menu return links should remain reachable.

The public file is the original self-contained export. No claim is made that it provides automated tests or a conventional source-code history.
