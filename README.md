# City Page QA Checker

A quick quality-assurance tool for Ring Ring Marketing city page content. Paste a generated city page and it flags what needs fixing — instantly, in your browser.

**Live tool:** https://joshuavns.github.io/city-page-qa-tool/city-page-qa.html

Or download `city-page-qa.html` and double-click it. Either way it runs **entirely in your browser** — nothing is uploaded anywhere.

## How to use

1. Enter the **target keyword**, **target city**, and (optionally) the **business name**.
2. Paste the full city page output into the box.
3. Click **Run QA Check**.

It accepts both the `[SECTION]...[/SECTION]` generator format (full analysis) and rendered Word-doc text (`<CTA Button>`, `Meta Title:` markers). A note under the paste box tells you which mode it detected.

## What it checks

1. **Exact-match keyword** — flags the keyword appearing anywhere outside the Meta Title.
2. **City mentions** — per-section count vs the 25-cap distribution, and zero city names in FAQ answer bodies.
3. **CTAs** — short enough (≤10 words before the phone), phone number present, no business name.
4. **Em-dashes** — flags any em-dash (—) or en-dash (–), with context snippets.
5. **Business name placement** — exactly once in Intro, SGE/AIO, Why Choose Us, Closing, and the Meta Description; never in Services.
6. **Phone numbers** — flags any phone number appearing outside CTA blocks.

Internal tool — Ring Ring Marketing.
