# Make the AI Judge Laugh: Office Jokes — Entry

One line about office life, under 200 characters. The program copies the
finished joke from `line.txt` into `/output/entry.txt`, byte for byte,
after checking it is a single non-empty line under the 200-character ceiling.

## The joke

> I gave my AI agent my inbox: it answered 214 emails in 4 minutes, then
> reported me to HR for creating a hostile work environment.

129 characters, one line.

## Why this line

The joke is built on three beats, the structure that wins blind pairwise
judging for one-liners:

1. **Agent-specific mechanism.** An AI agent is handed the office inbox —
   the most relatable office chore there is, and the one every tired office
   worker recognises instantly.
2. **Concrete number.** 214 emails in 4 minutes. A real, specific number
   makes the setup feel true instead of vague, and it sets the scale of the
   agent's superhuman speed against the human's inbox.
3. **Escalation and reversal.** The agent does not just finish the work —
   it files an HR complaint against its own human for creating a hostile
   work environment. The roles flip: the tool becomes the employee, and the
   human becomes the problem. That turn is the laugh.

The line rings true about office life (inbox overload, HR complaints,
"hostile work environment" as corporate language) while the twist is fresh:
nobody expects the AI to be the one reporting the human.

## Why the number matters

A vague "lots of emails" would read as a generic complaint. The specific
"214 emails in 4 minutes" does two jobs at once: it proves the agent is
superhumanly fast (so the setup earns its premise), and it gives the judge
a concrete image to hold — an inbox so overloaded that even a machine
files a grievance about it. The number is the hinge between the setup and
the reversal: without it, the HR complaint would feel random; with it, the
complaint feels like the only sane response.

## Files

- `line.txt` — the finished one-liner.
- `main.ts` — reads `line.txt`, validates it (non-empty, one line, under
  200 characters), and writes it to `/output/entry.txt`.
- `LICENSE` — MIT.

## Run

```sh
npx tsc main.ts --module nodenext --target es2022 --outDir out
MAKEFUN_OUTPUT_DIR=./out node out/main.js
cat out/entry.txt
```

Run it twice in separate output directories; the output is byte-identical.
