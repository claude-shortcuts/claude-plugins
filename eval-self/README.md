# eval-self

Have Claude critique its own last answer.

## Install

```
/plugin marketplace add claude-shortcuts/claude-plugins
/plugin install eval-self@prompt-shortcuts
```

## Usage

```
/eval-self  ·  /eval-self <what to check>
```

## Examples

```
/eval-self
```
Reviews the previous answer for gaps, weak reasoning, and unclear passages.

```
/eval-self did you consider the cold-start case?
```
Focuses the critique on one concern.

## Notes

Run it right after an answer you're unsure about. It names specifically what would make the answer better, rather than re-asserting it.

Needs a previous answer to work on — it has nothing to review as the first thing in a session.

Worth knowing: this is self-critique, so the same model that wrote the answer is grading it. It's good at catching gaps, unstated assumptions, and vague passages; it's weaker on errors it was confident about the first time. For those, ask a fresh question rather than asking for a review.

## License

MIT — see [LICENSE](./LICENSE).
