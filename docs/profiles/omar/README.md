# Omar's humanization profile

Custom patterns and prose rules for patina, distilled from my bachelor's
thesis humanization pass (scrolang comprehension research). These guidelines
were developed while humanizing ~10 thesis chapters and benchmarking each
one with `patina-cli --score`.

## My AI-tells list (what I strip from prose)

- Em-dash parentheticals — the classic "— which ..." aside
- (i)/(ii)/(iii) enumerations inside running prose
- "First / Second / Third" symmetrical openers
- Hedge-stacks ("it could perhaps be argued that...")
- Meta-commentary ("we note it here for completeness", "One caveat deserves
  emphasis:")
- Latinate-over-Germanic verbs ("underwrites" → "grounds")
- The "X is what makes Y do Z" construction

## Scoring bands I use (patina-cli --score)

- 0–15: human — target for abstract, intro, conclusion
- 15–30: mostly human — acceptable for technical chapters (math/code-dense
  prose scores structurally higher and resists reduction without changing
  meaning)
- 30+: mixed — unacceptable; structural AI-tells remain

## Editing lock for humanized prose

The source of truth for these rules is the thesis vault's CLAUDE.md
(humanization lock). Core principle: **after a text is humanized, agents
must not silently rewrite it for style, register, or "clarity"** — only
factual corrections, math-notation fixes, cross-reference updates,
consistency fixes, and code bugfixes are permitted without explicit author
approval. Awkward-looking prose is flagged to the author, never "fixed"
behind their back.
