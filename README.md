# Lucy — ADTC 2026 Submission Template

This is the submission repository for **Lucy** in the **Africa Deep Tech Challenge 2026** (Laptop LLM / Autonomous AI Agents track).

---

## 🚀 About Lucy

**Main Repository:** [github.com/Calvaryyy/lucy](https://github.com/Calvaryyy/lucy)

### What is Lucy?
Lucy is an autonomous AI agent and elite coding assistant engineered to run 100% offline on low-resource, commodity hardware (specifically targeting an 8GB RAM laptop with integrated graphics). Built with a Tauri 2 (Rust) core and backed by a size-optimized `llama.cpp` runtime, Lucy operates locally without relying on external cloud APIs or persistent internet connectivity.

### What Problem Does Lucy Solve?
In many African developer ecosystems, access to modern AI coding assistants is bottlenecked by unreliable internet connectivity and high, recurring API subscription costs. High-performing cloud agents are often inaccessible for students, independent researchers, and developers in remote or bandwidth-metered environments.

Lucy solves this by delivering reliable, agentic tool usage directly on budget hardware:
- **Offline Autonomy:** Plans multi-step dev tasks, inspects repositories, edits files, executes local CLI commands, and verifies tool actions completely offline.
- **Strict Grammar Enforcement:** Utilizes dynamic context-free grammar decoding paired with a post-hoc verification loop to ensure reliable function calling on small local models (~100% grammar validity rate).
- **RAM-Conscious Architecture:** Uses native webview rendering, SQLite vector storage (`sqlite-vec`), and a strict hierarchical context window management model to stay under strict memory ceilings.

---

## ✅ Submission Checklist

All required criteria have been verified and satisfied:

- [x] Repository is public on GitHub
- [x] `metadata.json` is fully filled in with no default placeholder values remaining
- [x] `metadata.json` contains exactly 2 domain-specific test prompts
- [x] `download_model.sh` successfully downloads the model weight file to `model/`
- [x] The model file is a valid GGUF format (`.gguf`)
- [x] `.gitignore` properly excludes `model/*.gguf` from version control
- [x] `REPORT.md` is completed with full architecture details and profiler benchmark metrics
- [x] `bash download_model.sh` runs idempotently without errors
- [x] The agent operates 100% offline with zero outbound network calls during execution

---

## 📁 Required File Structure
