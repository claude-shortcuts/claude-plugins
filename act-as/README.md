# act-as

Answer from a named role's seat.

## Install

```
/plugin marketplace add claude-shortcuts/claude-plugins
/plugin install act-as@prompt-shortcuts
```

## Usage

```
/act-as <role>: <question>
```

## Examples

```
/act-as CFO: should we fund a second data center this year?
```
Answers with a CFO's priorities — payback period, opex vs capex — and a CFO's blind spots.

```
/act-as skeptical customer: here's our new pricing page
```
Pushes back the way a wary buyer would.

## Notes

Brings the role's priorities and blind spots, not just its vocabulary. Naming a role you want challenged ("skeptical customer", "security reviewer") tends to be more useful than naming a friendly one.

## License

MIT — see [LICENSE](./LICENSE).
