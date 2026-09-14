# compare

Put options side by side on the same criteria.

## Install

```
/plugin marketplace add claude-shortcuts/claude-plugins
/plugin install compare@prompt-shortcuts
```

## Usage

```
/compare <a> vs <b>
```

## Examples

```
/compare Redis vs Memcached for session storage
```
Same criteria applied to both, differences called out.

```
/compare renting vs buying CI runners
```
Skips the criteria where they're basically the same.

## Notes

Compares options you describe. It does not read your files or git history — paste in anything it needs to see.

## License

MIT — see [LICENSE](../LICENSE).
