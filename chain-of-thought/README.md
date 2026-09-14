# chain-of-thought

Work a hard problem in visible steps.

## Install

```
/plugin marketplace add claude-shortcuts/claude-plugins
/plugin install chain-of-thought@prompt-shortcuts
```

## Usage

```
/chain-of-thought <problem>
```

## Examples

```
/chain-of-thought if we cut cache TTL to 30s, what breaks first?
```
States the givens, reasons forward a move at a time, then concludes.

```
/chain-of-thought why would this deadlock only under load?
```
Shows the intermediate steps so you can check them.

## Notes

Useful when you need to audit the logic rather than trust a conclusion. This shapes the visible answer into explicit steps; it does not expose the model's internal reasoning.

## License

MIT — see [LICENSE](../LICENSE).
