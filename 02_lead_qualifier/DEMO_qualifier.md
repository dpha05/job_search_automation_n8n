# 🧠 Phase 2: Lead Qualification 
**Hybrid AI-driven scoring engine with semantic anchors and state-machine reliability.**

<br>

### 📊 Highlights
* **71% Rejection filter:** Two-stage hybrid filtering (AI + Cosine Similarity) auto-rejects low-level leads before deep-dive processing.
* **Dual-Strategy Scoring:** Combines high-context **Gemini 3.0 Flash** reasoning for core pillars with **Llama 4 (Groq)** boolean extraction for zero-hallucination benefit checks.
* **Lazy-Loading Optimization:** "Lean Payload" architecture strips 1536D vectors during transit to optimize memory, fetching them only during final database-side similarity math.
* **Self-Healing State Machine:** Automated daily sync identifies leads in transient statuses (e.g., `passed_title`) to ensure 100% fault tolerance and zero data loss.

<br>

---

<br>

![](https://github.com/dpha05/job_search_automation_n8n/raw/main/02_lead_qualifier/assets/demo.png)

<br>

---

<br>

### 🎥 Video Walkthrough (100 Seconds)

[![Video Walkthrough Preview](https://img.youtube.com/vi/iOiFAwF-i9M/0.jpg)](https://www.youtube.com/watch?v=iOiFAwF-i9M)

<br>

---

<br>

### 🖼️ n8n Workflow Screenshots

**Stage 1: Technical Filter:**
![Technical Filter Preview](assets/screenshot_reject.png)

<br>

**Stage 2: 3-Branch Scoring Engine:**
![Scoring Engine Preview](assets/screenshot_score.png)

<br>

**Global Anchor Management:**
![Global Anchors Preview](assets/screenshot_anchor.png)

<br>

**Status Sync:**
![Status Sync Preview](assets/screenshot_sync.png)

<br>

---

<br>

### 📂 Technical Documentation
* [**Raw JSON Workflows**](workflows/)
* [**Detailed Technical README**](../README.md)

<br>

---

### ✅ Next steps
* **Auto-Apply Integration:** Researching automated "Quick Apply" triggers for roles hitting the 95th percentile "Rare" score.
* **Portfolio Matching:** Adding a sub-flow to compare specific job requirements against a vectorized database of my past projects to generate tailored highlights.
* **Multi-Persona Anchors:** Expanding the Global Anchor system to allow switching between different career personas (e.g., Technical Architect vs. Product Lead).
* **Local LLM Integration:** Testing Ollama integration for the Boolean branch to move the 33-question check entirely offline, further reducing API costs.
* **Enhanced Notifications:** Refining Pushover alerts to include a "Deep Link" directly to the job URL and a 1-sentence AI summary of why it was marked as 'Rare'.

<br>

---
[← Return to Portfolio](https://linktr.ee/dpha05)
