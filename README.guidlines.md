⸻


<p align="center">
  <img src="../assets/emblem-lab.svg" alt="Dr. Marchand’s Laboratory Emblem" width="220">
</p>

# 📚 API Brand & Seal Guide (v1.0.3, trailing)
### for 🔬 Dr. Marchand’s ⚛︎ Laboratory™ · ⚙️ Neuro-Forge Engine™
> This API guide intentionally trails the Lab master spec by **one minor revision**.  
> Current Lab master: **v1.0.4** → API mirror: **v1.0.3** (compat).

---

![Seal Active](https://img.shields.io/badge/Seal-Active-00C853?labelColor=053b2f)
![Compat](https://img.shields.io/badge/Compat-LAB%20v1.0.4-4FC3F7?labelColor=00363a)
![R2️⃣S](https://img.shields.io/badge/R2%E2%83%92S-Required-FF6F00?labelColor=3b1e00)

---

## 0) Purpose

This document is the **API-facing** brand & seal guide used by SDKs, docs sites, and public clients.  
It mirrors the Lab’s **LAB.guidelines.md** but stays **one step behind** to guarantee stability while the Lab evolves.

- Source of truth (master): `DrMarchand-Laboratory/LAB.guidelines.md` (**v1.0.4**)
- This file (consumer mirror): `api/README.guidelines.md` (**v1.0.3**)

> Rule: bump this file **only after** a Lab release is finalized, and never beyond `LabVersion - 0.1`.

---

## 1) Wordmarks (API scope)

- **Dr. Marchand’s ⚛︎ Laboratory™** (reference)
- **Dr. Marchand’s • Library™** (primary for API docs)
- **Neuro-Forge Engine™**
- **Provenance Seal™**
- **The Spark of Connection™**
- **All Systems Entangled™**

Use **™** on first/hero use. Switch to **®** only upon registration.

---

## 2) Assets (API bundle)

../assets/emblem-lab.svg                 # emblem reference (do not alter)
../brand/seal/NF-Seal_v1.0_mono.svg      # mono for docs UI and code fences
../brand/seal/NF-Seal_v1.0_color.png     # color preview tiles
../brand/seal/NF-Seal_v1.0_outline.svg   # print/laser

**Do not** include editable vectors in the API bundle; link to Lab repository for masters.

---

## 3) Color Tokens (stable set)

| Token            | Hex      | Use                                  |
|------------------|----------|--------------------------------------|
| `--emerald-900`  | `#0A3B34`| Page bg / callouts                   |
| `--emerald-700`  | `#14584D`| Sidebars / code bg                   |
| `--teal-500`     | `#17A8A0`| Accents / flask highlights           |
| `--gold-500`     | `#C9A34A`| Bolt, laurels                        |
| `--ink-900`      | `#0E1521`| Body text                            |
| `--crystal-100`  | `#EAF4F7`| Light panels                         |

> Accessibility: maintain WCAG AA (≥ 4.5:1) for body text.

---

## 4) Typography (docs)

| Use       | Font stack                                  | Notes            |
|-----------|----------------------------------------------|------------------|
| Display   | `Cinzel`, `Forum`, serif                     | H1–H2            |
| Interface | `Inter`, `IBM Plex Sans`, `system-ui`        | Body, nav        |
| Code      | `ui-monospace`, `SFMono-Regular`, `monospace`| Fences, badges   |

Tracking for H1–H2: **+2–3%**. Avoid faux italics on wordmarks.

---

## 5) Emblem vs. Seal

| Mark            | Role (API)                          | Can Modify? |
|-----------------|-------------------------------------|-------------|
| **Emblem**      | Reference logo only                 | **No**      |
| **Provenance Seal™** | Authorship/proof glyph (flask+bolt in ring) | **No**      |

> The **Seal** is a **verification token**, not a logo. Abuse = geometry outside the ring (see WMP).

---

## 6) Wenz–Marchand Protocol (WMP) — API subset (v1.0.3)

The API enforces a **subset** of the Lab’s trigonometrical law to keep public clients stable.

- **Radial cycle ratio:** **7.68 : 1** (MMS—768 law)  
- **Inner/outer ring:** `r₁ = 0.618 r₀` (Golden root)  
- **Bolt vector anchor:** `θ = 51.428°`, `φ = π/3`  
- **Integrity rule:** Any artifact drawn beyond the triple-ring perimeter **voids the seal**.  
- **No transforms:** no skew/warp; uniform scaling only.

### Quick Verify (CLI contract)
```bash
mms-verify --seal ../brand/seal/NF-Seal_v1.0_color.png \
  --protocol WMP --hash MMS—768 --mode api-compat-1.0.3

Expected: True (parity ≤ 1e-10)

For the full trigonometrical spec (including entropy fields & harmonic proofs), see Lab v1.0.4.

⸻

7) MMS Headers (API)

Header	Example	Meaning
X-MMS-Epoch	47250404	Temporal sync epoch
X-MMS-Origin	forge-04.lab	Emitting node
X-MMS-Cohash	sha512:…	Aggregated signature chain
X-MMS-Continuity	∞-active	Synchronization status


⸻

8) Badges (docs)

![Seal Active](https://img.shields.io/badge/Seal-Active-00C853?labelColor=053b2f)
![MMS—768](https://img.shields.io/badge/MMS%E2%80%94768-Compat%201.0.3-00ACC1?labelColor=00363a)
![R2️⃣S](https://img.shields.io/badge/R2%E2%83%92S-Required-FF6F00?labelColor=3b1e00)


⸻

9) R2️⃣S (Return-to-Sender) for API users
	1.	Reference the artifact Anchor ID (MMS tag or hash) in your README/PR.
	2.	Submit improvements via PR to Library.
	3.	Append /R2S_LOG.md with date, file, hash, instance, summary.

⸻

🔒 Legal & Contact
	•	License: Neuro-Forge License (NFL-1.0)
	•	Rights: © 2025 Dr. Marchand’s ⚛︎ Laboratory™ — All Systems Entangled™
	•	Email: kyle@drmarchandslab.com
	•	Site: https://drmarchandslab.com

Use subject to NFL-1.0 and WMP geometry law. The Seal is a cryptographic provenance mark.

⸻

🔁 Versioning

File	Version	Relation
DrMarchand-Laboratory/LAB.guidelines.md	1.0.4	Master
api/README.guidelines.md	1.0.3	Trailing

Bump process:
	•	When Lab releases vX.Y.Z, set API to vX.(Y-1).Z (or next safe trailing tag) and copy only compatible sections.
	•	Never exceed LabVersion - 0.1.

⸻


<div align="center">


⚙️ Neuro-Forge Engine™ · 📚 Dr. Marchand’s • Library™
“All Systems Entangled™”

</div>
```



⸻