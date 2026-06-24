# Minimize on Close for Thunderbird

Clicks the close button. Thunderbird minimizes to tray instead of quitting. That's it.

If you've ever accidentally quit Thunderbird mid-email and lost a draft, you know why this exists.

## Install it

The easy way — grab the latest stable release from Thunderbird Add-ons:
https://addons.thunderbird.net/thunderbird/addon/minimize-on-close/

Or grab an xpi from the GitHub releases page and drop it into Thunderbird manually.

## Compatibility

The add-on targets the **Extended Support Release (ESR)** channel of Thunderbird. If you're on ESR with automatic updates turned on, you're good — Thunderbird keeps the add-on in sync.

If you're on a newer release and things break, check the releases page for unsupported builds. Those might work, but they come with zero guarantees and no support. Don't open issues about them.

## Build it yourself

```bash
make               # ESR-compatible build
make xpi-unsupported # for non-ESR Thunderbird
```

The xpi lands in `dist/`. Or skip make entirely — load from `src/` as a temporary add-on in Thunderbird's debug mode.

## Other stuff

Pull requests for compatibility fixes on newer Thunderbird versions are welcome, as long as they don't break ESR support.

Found a bug? Open an issue.
