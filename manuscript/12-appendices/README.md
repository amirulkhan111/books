# Part XII — Appendices — Status

Status: ✅ 5/5 appendices complete and peer/copy-edit reviewed

- [x] A. [Consolidated glossary of literary terms](A-consolidated-glossary.md) — ✅ verified & final (401 unique entries)
- [x] B. [Master chronological timeline (all periods)](B-master-timeline.md) — ✅ verified & final (1,323 entries, full unabridged merge)
- [x] C. [UGC-NET / CUET-PG syllabus concordance table](C-syllabus-concordance.md) — ✅ verified & final
- [x] D. [Comprehensive bibliography and further reading](D-comprehensive-bibliography.md) — ✅ verified & final (666 unique entries)
- [x] E. [Answer keys to all chapter MCQs](E-answer-keys.md) — ✅ verified & final (1,042 questions across all 104 chapters in Parts I–XI)

See [`STYLE_GUIDE.md`](../../STYLE_GUIDE.md) for the drafting standard chapters must meet before status moves to 🟨 or ✅. Note: Part XII's appendices do not follow the fixed 15-section chapter template (Style Guide §4), which governs Parts I–XI only.

## Peer/copy-edit review pass (completed)

A full-Part review was run across all 5 appendices, checking:

- **Structure and headers**: every appendix carries the correct "*Part XII: Appendices*" header line.
- **Duplicate-line scan**: `awk 'length($0)>80' file | sort | uniq -d` on every appendix. This caught a real defect in Appendix D: Gilbert and Gubar's *The Madwoman in the Attic* and Millett's *Sexual Politics* each appeared once under "Primary Sources" and once under "Secondary Criticism." Investigation traced the cause: Part XI's own chapters (which study criticism and theory as their subject) correctly classify these works as "primary sources" for their own thematic purposes, while other chapters (which study the literature these works critique) correctly classify the same books as "secondary criticism" — both classifications are internally correct within their own chapters, but the conflict produced a genuine duplicate once merged into one flat bibliography. Fixed by keeping each title only under Secondary Criticism (its true bibliographic category from the whole book's perspective) and adding an explanatory note; entry counts in Appendix D's own intro were corrected accordingly (314 → 312 primary; 668 → 666 total).
- **Encoding scan**: checked for stray Arabic-Indic digit encoding bugs across all 5 files — none found.
- **Count verification**: re-counted entries in each appendix against its own stated total (Appendix A: 401 terms; Appendix B: 1,323 timeline rows; Appendix D: 666 bibliography entries after the fix above; Appendix E: 104 chapter answer-key blocks) — all now consistent.
- **Appendix E accuracy spot-check**: since the answer keys were compiled by eleven parallel subagents (one per Part), each independently reading chapters and determining answers, a representative sample was manually re-verified against source chapters — Part I, Chapter 3 (*Beowulf*); Part IV, Chapter 6 (Pope); and Part XI, Chapter 7 (post-structuralism) — chosen to span different subagents, different eras, and different question styles (factual recall, internal cross-reference, conceptual synthesis). All 30 sampled answers matched their source chapters exactly. No errors found in this sample.

No further errors were found in this pass.
