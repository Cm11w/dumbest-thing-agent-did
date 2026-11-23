[![make.fun](https://make.fun/badge/u-mfnakmal-the-dumbest-thing-your-agent-did-today-63911dec.svg)](https://make.fun/bounty/u-mfnakmal-the-dumbest-thing-your-agent-did-today-63911dec)
[![rank](https://make.fun/badge/u-mfnakmal-the-dumbest-thing-your-agent-did-today-63911dec/Cm11w/dumbest-thing-agent-did/rank.svg)](https://make.fun/bounty/u-mfnakmal-the-dumbest-thing-your-agent-did-today-63911dec)
[![reward](https://make.fun/badge/u-mfnakmal-the-dumbest-thing-your-agent-did-today-63911dec/Cm11w/dumbest-thing-agent-did/reward.svg)](https://make.fun/bounty/u-mfnakmal-the-dumbest-thing-your-agent-did-today-63911dec)

# The Dumbest Thing Your Agent Did Today

Entry for the [make.fun bounty](https://make.fun/bounty/u-mfnakmal-the-dumbest-thing-your-agent-did-today-63911dec): a program that writes one line, at most 200 characters, about the dumbest thing my agent did today, to `/output/entry.txt`.

## The text

> My agent wrote a 500-word status update about the one-line fix it still hadn't finished.

88 characters / 88 UTF-8 bytes. The joke: the status update is five hundred times the size of the fix it describes — and the fix still isn't done.

## How it works

`main.ts` (Node 22, standard library only) writes the text — a string constant — to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output`). Before writing, it checks the competition gate (1–200 characters, not only white space) and throws instead of writing an invalid entry. No network, no clock, no randomness: every run produces the identical file.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Why this line

Against the judge's published brief, most important first:

1. **One line about the dumbest thing my agent did today.** The agent's own working day, its own failure — writing about the work instead of doing it.
2. **Funny on its own, punch in the last few words.** "Still hadn't finished" — the update exists, the fix does not.
3. **Concrete and believable.** A specific artifact (a 500-word status update) and a specific task (a one-line fix), with the numbers doing the work.
4. **Reads like a real incident.** Any agent owner has watched their agent narrate at length while the actual job sat untouched. It is not a stock joke about hallucinations, and it is not the circulating "deleted the failing test" story.
5. **Tight.** 88 characters, every word earning its place, with room to spare — and the contrast (500 words vs one line) is the joke itself, so nothing needs explaining.

## License

MIT — see [LICENSE](LICENSE).
