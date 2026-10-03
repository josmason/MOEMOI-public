# Pre-Publication Quality Review

*Run these 5 checks before flipping the repo to public. Takes approximately 3 minutes.*

---

## Check 1 — Claim count consistent across index and register

```bash
# Should return the same number from both files
grep -c "^| C[0-9]\|^- \*\*C[0-9]" MOEMOI_Claims_Index.md
grep -c "ADOPTED" MOEMOI_Claims_Register.md
```

Expected: Claims Index count matches the total ADOPTED claims in the register.

---

## Check 2 — No ARCHIVED claims in the public-facing index

```bash
grep -n "ARCHIVED" MOEMOI_Claims_Index.md
```

Expected: no output (zero archived claims in the public index).

---

## Check 3 — Preprint PDF present and non-zero

```bash
ls -lh MOEMOI_Preprint_Draft_v1.pdf
```

Expected: file exists, size approximately 170-200 KB.

---

## Check 4 — CITATION.cff complete (title and ORCID populated)

```bash
grep -n "title:\|orcid:\|family-names:" CITATION.cff
```

Expected: title line is populated, orcid line contains a real ORCID (format: 0000-0000-0000-0000), family-names is "Mason".

---

## Check 5 — Fold integrity (no stale internal references in canonical)

```bash
# Run from the repo root (MOEMOI 31.5.26/)
python3 tools/los_skill/scripts/fold_integrity_check.py 2>/dev/null | tail -3
```

Expected: "PASS -- no stale references found in public repo"

---

## After passing all 5 checks

Go to github.com/josmason/MOEMOI-public → Settings → Change repository visibility → Make public.

This is A110 in your action list.

---

*B32763 | W1088-PRODUCT | 2026-08-05 | AI-authored. Replaces the internal-marker placeholder from B31803.*
