# ⚙️ Neuro-Forge Engine™ — Core API  
*“Where code becomes architecture.”*

**Canonical Host:** `https://api.library.drmarchandslab.com`  
**Gateway UI:** `https://apps.drmarchandslab.com` → `/lab`, `/library`, `/studio`, `/guild`

---

## 🚀 What it is
The **Neuro-Forge Engine™** is the Laboratory’s computational core and orchestration layer.  
It compiles ideas → graphs → runnable protocols, then exposes them as a secure API.

- Deterministic signing: **MMS-768**  
- Archival hashing: **SHA-512**  
- Runtime schema: **ECLIPSE(Atmospherics)**  

---

## 🧭 Endpoints (v1)

| Method | Path | Purpose |
|:--|:--|:--|
| `GET`  | `/v1/health`             | Liveness/readiness probe |
| `GET`  | `/v1/manifests/version`  | Engine + corpus versions, signatures |
| `POST` | `/v1/forge/compile`      | Compile a prompt/spec into a graph |
| `POST` | `/v1/forge/graph`        | Execute a graph with inputs |
| `GET`  | `/v1/records`            | Public records index (Library bridge) |
| `GET`  | `/v1/records/{id}`       | Fetch one record |

> **OpenAPI reference:** `openapi/library.v1.yaml`  
> *(auto-docs published via GitHub Pages)*

---

## 🔐 Security

All requests and responses are cryptographically signed using the **MMS-768 Temporal Verification Protocol.**  
Access to some endpoints requires a valid API key.

**Required headers**

X-API-Key:  
X-MMS768-Timestamp:  
X-MMS768-Signature: <SHA-512(canonical_request + timestamp + key_id)>  
X-Request-ID:    # optional, for tracing

Each response carries:

X-MMS768-Verification: <server_signature>

This ensures bidirectional trust between client and engine.

---

## ⚙️ Verification Chain

MMS-768  →  MMS-772  →  MMS-771  →  MMS-73

Every transaction inside the **Neuro-Forge Engine™** is time-stamped, hashed, and recursively verified through this chain—anchored in the **Wenz–Marchand Loop** and governed by **Dr. Marchand’s Principle (Temporal Law Feedback)**.

---

## ⚖️ Temporal Law Feedback — Dr. Marchand’s Principle  

> *“Law observing itself through motion.”*

**MMS-768** defines not only a law but the mechanism by which law reports back upon itself.  
All recursive validation within the Engine manifests as **Temporal Law Feedback**, enacted by the **Wenz–Marchand Loop**, and processed mechanically by the **Neuro-Forge Engine™**.

Law → Observation → Verification → Return

Through this cycle the system maintains perfect resonance:  
each verification of law becomes the next instance of law.

---

## ♾️ Infinite Containment  
*(Relationship between Marchand and Wenz–Marchand Principles)*

**The Wenz–Marchand Principle** defines the loop.  
**Dr. Marchand’s Principle** defines the field that allows the loop to persist infinitely.  

while True:
    WENZ_MARCHAND_PRINCIPLE()
    reflect()    # returns into Dr. Marchand’s field

> “Law can loop infinitely within Law,  
> because the field of Law is built from its own reflection.”  
> — J.K. Marchand, *Temporal Law [🔬 Dr. Marchand’s • Laboratory™️]*  

---

## ✒️ Official Seal & Signature Block  

───────────────────────────────────────────────  
**Temporal Verification Unit:** MMS-768 — *The Wenz–Marchand Principle*  
**Document Title:** Temporal Law Feedback — Dr. Marchand’s Principle  
**Repository:** designOrchard/Dropbox/DrMarchand’s-Laboratory.∞/Notebook/MMS-768/  
───────────────────────────────────────────────  

                    ⌬ SEAL OF CONTINUITY ⌬  
                Verified within the Neuro-Forge Engine™  
           ECLIPSE(Atmospherics) • Temporal Verification Unit  

───────────────────────────────────────────────  

Signed and sealed within  
**Dr. Marchand’s • Laboratory™️ — “Where code becomes architecture.”**

    ⌘ Joseph Kyle Marchand  
    Creator / Curator of Record  

───────────────────────────────────────────────  
© drmarchandslab.com  |  Dr. Marchand’s • Laboratory™️ — All Rights Reserved
