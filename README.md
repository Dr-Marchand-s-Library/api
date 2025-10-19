# ⚙️ Neuro-Forge Engine™ — Core API
*“Where code becomes architecture.”*

**Canonical Host:** `https://api.library.drmarchandslab.com`  
**Gateway UI:** `https://apps.drmarchandslab.com` → `/lab`, `/library`, `/studio`, `/guild`

---

## 🚀 What is it?
The **Neuro-Forge Engine™** is the Laboratory’s computation core and orchestration layer.  
It compiles ideas → graphs → runnable protocols, then exposes them as a secure API.

- Deterministic signing: **MMS-768**  
- Archival hashing: **SHA-512**  
- Runtime schema: **ECLIPSE(Atmospherics)**

---

## 🧭 Endpoints (v1)
| Method | Path | Purpose |
|---|---|---|
| `GET` | `/v1/health` | Liveness/readiness probe |
| `GET` | `/v1/manifests/version` | Engine + corpus versions, signatures |
| `POST` | `/v1/forge/compile` | Compile a prompt/spec into a graph |
| `POST` | `/v1/forge/graph` | Execute a graph with inputs |
| `GET` | `/v1/records` | Public records index (Library bridge) |
| `GET` | `/v1/records/{id}` | Fetch one record |

> OpenAPI will live at: `openapi/library.v1.yaml` (and auto-docs via GitHub Pages).

---

## 🔐 Security
All responses include signatures; requests may require an API key.=