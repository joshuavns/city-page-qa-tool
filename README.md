# City Page QA Checker

A quick quality-assurance tool for Ring Ring Marketing city page content. Upload or paste a generated city page and it flags what needs fixing — instantly, in your browser.

**Live tool:** https://joshuavns.github.io/city-page-qa-tool/

Or download `index.html` and double-click it. Either way it runs **entirely in your browser** — nothing is uploaded anywhere.

## How to use

1. **Open the tool:** go to https://joshuavns.github.io/city-page-qa-tool/
2. **Fill in the fields at the top:**
   - **Target keyword** — the exact keyword phrase for the page (e.g. *funeral home and cremations in Dearborn, MI*)
   - **Target city** — just the city (e.g. *Dearborn*)
   - **Business name** — optional, but fill it in to check name placement and CTAs
3. **Add the content** one of two ways:
   - **Easiest:** click **Load a file** and pick the page's **.docx**, or
   - **Paste** the page text into the big box.
4. **Click Run QA Check.** (If you uploaded a file, it runs automatically.)
5. **Read the results** on the right. Each check is color-coded:
   - 🟢 **PASS** — all good
   - 🟡 **REVIEW** — worth a look
   - 🔴 **ISSUES** — needs fixing

   Open any flagged check to see the exact problem text and a **Fix:** line telling you what to change.
6. **Make the fixes** in your document, then re-run to confirm everything turns green.

Schema blocks and image details (Alt Text / File Name / Download) are ignored automatically, so you don't need to remove anything first.

**Input formats:** the tool accepts a `.docx` upload, pasted Word-doc text, or the `[SECTION]...[/SECTION]` generator format. The section-tagged format gives the most precise per-section breakdown; a note under the paste box tells you which mode it detected.

## What it checks

1. **Exact-match keyword** — flags the keyword appearing anywhere outside the Meta Title.
2. **City mentions** — per-section count vs the 25-cap distribution, and zero city names in FAQ answer bodies.
3. **CTAs** — short enough (≤10 words before the phone), phone number present, no business name.
4. **Em-dashes** — flags any em-dash (—) or en-dash (–), with context snippets.
5. **Business name placement** — exactly once in Intro, SGE/AIO, Why Choose Us, Closing, and the Meta Description; never in Services.
6. **Phone numbers** — flags any phone number appearing outside CTA blocks.
7. **HTML tags** — flags unbalanced/malformed markup: a `<CTA Button>` without its `</CTA Button>`, unclosed headings, or typos like `</3>` instead of `</h3>`.

Internal tool — Ring Ring Marketing.
