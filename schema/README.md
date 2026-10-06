# schema

Extract named fields as machine-readable data.

## Install

```
/plugin marketplace add claude-shortcuts/claude-plugins
/plugin install schema@prompt-shortcuts
```

## Usage

```
/schema <fields>: <source>
```

## Examples

```
/schema name, email, company: <paste signatures>
```
Returns just the structured data.

```
/schema title, severity, owner: <paste an incident log>
```
Fills exactly the fields you named.

## Notes

Output is JSON, key-value, or a filled template with no prose around it, so it can be piped or parsed. Nothing extra, nothing missing.

## License

MIT — see [LICENSE](./LICENSE).
