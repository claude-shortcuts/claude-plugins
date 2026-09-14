# prompt-shortcuts

Fifteen small prompt-shaping plugins for Claude Code. Each one is a single skill that
changes *how* Claude answers — the length, the structure, the vocabulary, the point of view —
without you having to spell it out every time.

None of them read your files, run commands, or reach the network. They shape a response and
nothing else.

## Install

```
/plugin marketplace add claude-shortcuts/claude-plugins
```

Then install whichever you want:

```
/plugin install tldr@prompt-shortcuts
```

## The plugins

### Length and density

| Plugin | What it does |
|---|---|
| [`briefly`](./briefly) | A short answer instead of a full explanation — no preamble, no padding |
| [`tldr`](./tldr) | Compress something long into a one-line takeaway plus the points that matter |
| [`exec-summary`](./exec-summary) | Recast something long for whoever has to make a call on it |

### Structure

| Plugin | What it does |
|---|---|
| [`format-as`](./format-as) | Shape the answer into a table, email, memo, FAQ, or outline |
| [`checklist`](./checklist) | Checkbox items, one concrete action each |
| [`step-by-step`](./step-by-step) | Ordered instructions with nothing assumed between steps |
| [`schema`](./schema) | Named fields as JSON or a filled template, no prose around it |
| [`compare`](./compare) | Options side by side on the same criteria |

### Voice and framing

| Plugin | What it does |
|---|---|
| [`tone`](./tone) | Set the register — formal, blunt, warm, urgent — without changing the content |
| [`jargon`](./jargon) | Dial technical vocabulary up or down, substance untouched |
| [`audience`](./audience) | Frame the explanation for a specific reader |
| [`act-as`](./act-as) | Answer from a named role's seat, with its priorities and blind spots |

### Reasoning and scrutiny

| Plugin | What it does |
|---|---|
| [`chain-of-thought`](./chain-of-thought) | Work a hard problem in visible steps |
| [`pitfalls`](./pitfalls) | Stress-test a plan: what breaks, why, and the early signal |
| [`eval-self`](./eval-self) | Have Claude critique its own last answer |

## Picking between the close ones

A few of these overlap, so:

- **`tldr` vs `exec-summary`** — `tldr` is for getting the gist yourself; `exec-summary` is for
  someone who has to decide something.
- **`checklist` vs `step-by-step`** — `step-by-step` is a process you follow once, front to back;
  `checklist` is something you verify repeatedly.
- **`jargon` vs `audience`** — `jargon` changes only the wording; `audience` changes what gets
  included at all.
- **`format-as` vs `schema`** — `format-as` is for humans reading it; `schema` is for something
  parsing it.

## Usage

Every plugin takes its input inline after the skills:

```
/tldr <paste something long>
/tone blunt: explain why this PR can't merge
/compare Redis vs Memcached for session storage
```

Each plugin's own README has more examples.

## License

MIT — see [LICENSE](./LICENSE).
