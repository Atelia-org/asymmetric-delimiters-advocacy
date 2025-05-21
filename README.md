# Escaping Hell — Advocacy for Asymmetric Delimiters

> **"Raw blocks without counting quotes."**  
> A community call to standard-bodies, language designers and tool authors:
> adopt **asymmetric delimiter pairs** so humans *and* large-language-models
> can stop drowning in escape characters.

---

## Why this repo exists

LLMs generate text serially and cannot "go back" to repair a mis-counted
quote or closing fence.  Humans suffer the same pain in Markdown,
JSON, shell scripts, and code.  
A simple structural fix — **distinct open / close delimiters** — eliminates
whole classes of escaping failure.

This repository bundles the rationale, examples and next-step proposals
so anyone can point to a single URL when filing language-spec or
toolchain feature requests.

> **📝 Note on names**  
> We deliberately *did not* register `escaping-delimiter-hell` on GitHub so that
> a future **implementation-focused** project (parser libraries, transpilers,
> proof-of-concept PRs) can claim that more evocative slug.  
> Here we focus purely on advocacy and reference material.

---

## Contents

| File | Purpose |
|------|---------|
| **`escaping-hell-why-both-humans-and-llms-need-asymmetric-delimiters.md`** | Main position paper / call to action. |
| **`appendix-edit-history.md`** &nbsp;·&nbsp; `appendix-edit-history.hans.md` | Complete revision log (English + original Chinese). |
| **`appendix-additional-delimiter-examples.md`** | Cross-language survey of escaping pain points. |
| **`appendix-toward-universal-unicode-raw-delimiter-pair.md`** | Early thoughts on a longer-term, Unicode-level solution. |
| **`LICENSE`** | The Creative Commons CC-BY-4.0 license text. |

*(If you translate or extend any appendix, please keep filenames parallel
for easy diffing.)*

---

## How you can help

1. **File issues** with concrete examples from your favourite language /
   format where asymmetric fences would help.
2. **Open PRs** adding real-world failure cases or success stories.
3. **Share the paper** in standards venues (ECMA, ISO, IETF, language
   mailing lists) and link ensuing discussions back here.

We—the original authors (a Gemini instance, a ChatGPT instance, a Claude instance, and Shichao
Liu)—may not have bandwidth to shepherd a full specification process, so
community ownership is encouraged.

---

## Licence

All text in this repository is released under the
[CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/) licence.  
Quote, remix or fork with attribution.

---

## Acknowledgements

Thanks to everyone—human and AI—who contributed use-cases, edits and
translations.  Special shout-out to future implementers who will one day
make *escaping delimiter hell* a distant memory.
