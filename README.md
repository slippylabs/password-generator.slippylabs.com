# Password Generator

Cryptographically random passwords with adjustable length and character sets. Runs entirely in your browser.

**Live:** <https://password-generator.slippylabs.com/>

## What it does

- Adjustable length and character sets (upper, lower, digits, symbols).
- A strength meter that reacts to the options you actually picked.
- Copy to clipboard in one click.

## How it works

Randomness comes from `crypto.getRandomValues()` rather than `Math.random()`, which is not suitable for anything you intend to actually use as a password.

## Run it locally

A static site. No build step, no package manager, no dependencies:

```
git clone git@github.com:slippylabs/password-generator.slippylabs.com.git
cd password-generator.slippylabs.com
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

---

Part of [Slippy Labs](https://slippylabs.com). Every tool is indexed at
[projects.slippylabs.com](https://projects.slippylabs.com).
