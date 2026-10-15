# Thesis chapters — humanization lock

The prose in this directory (`*.md`) has been humanized by the author. The humanization pass removed AI-tells: em-dash parentheticals, (i)/(ii)/(iii) lists inside prose, "First/Second/Third" symmetrical openers, hedge-stacks, meta-commentary ("we note it here for completeness", "One caveat deserves emphasis:"), Latinate-over-Germanic verbs ("underwrites" → "grounds"), and the "X is what makes Y do Z" construction.

## Rules for any future session editing these files

**Do not silently rewrite prose for style, register, or "clarity".** The current wording is the author's, even where it looks awkward to you.

**Permitted edits without explicit author approval:**
- Factual corrections (wrong number, wrong citation, wrong cross-reference)
- Math notation fixes (LaTeX rendering bugs, symbol errors)
- Cross-reference updates (section renumbering, broken links)
- Consistency fixes with the rest of the thesis (terminology unification)
- Bug fixes in any code/pseudocode blocks

**Forbidden without explicit author approval:**
- Rewriting sentences because they "could be clearer"
- Breaking or joining sentences for rhythm
- Replacing em-dashes the author left in (some are intentional)
- "Tightening" or "smoothing" prose
- Reformatting lists or enumerations
- Removing meta-commentary the author left in (some is intentional academic register)

**If you spot prose that looks awkward, AI-flavored, or wrong:** flag it in your reply to the author. Don't fix it silently. The author decides whether to humanize further.

## Verification

The author benchmarks humanization with `patina-cli --score`. Latest scores per chapter are in the commit history; the deterministic score is the trustworthy signal (the LLM commentary field hallucinates evidence and should be ignored). Score thresholds:
- 0–15: "human" band (target for abstract, intro, conclusion)
- 15–30: "mostly human" band (acceptable for technical chapters with math/pseudocode)
- 30+: "mixed" band (unacceptable; means structural AI-tells remain)

Chapters 2, 4, 6, 7 were the primary humanization targets. Chapters 3 and 5 are technical (math/code-dense) and have structurally higher scores that resist further reduction without changing meaning.
