# Website Changelog

All fact-check and content changes tracked here for cross-page reference.

---

## 2026-04-06 — Impact Cards & Blog Posts (index.html, posts/, news.html)

### Impact card links
- BharatSim: Global Headlines → `project.html?id=bharatsim`
- Cancer Diagnostics AI → `project.html?id=cancer-ascend`
- Oxford Fellowship → `project.html?id=pollen-project`
- IndiaMediaLens → `project.html?id=indiamedialens`
- RedBrick Hacks III → `posts/2026-02-redbrick-hacks-iii.html`
- Government Recognition → `project.html?id=cs-pedagogy`

### Blog posts created
- `posts/2026-02-redbrick-hacks-iii.html` — RedBrick Hacks III (Feb 6-8, 2026). Source: RBH III Report PDF + Q4 Report. Images extracted from PDF. Prize cheque image excluded (shows financial data). Humanizer pass applied.
- `posts/2026-03-wicscon-3.html` — Updated: removed sponsors, team names, internal details. Hero cropped. Humanizer pass applied. Source: WiCSCon3 documentation PDF.
- `posts/2026-03-acm-compute-2026.html` — Updated: removed Context/Related sections. Added photos from ACM Compute Pictures folder. Source: Q4 Report.

### News & Events page (news.html)
- Added 3 Q4 events to timeline (WiCSCon 3.0, ACM COMPUTE 2026, ITiCSE papers)
- RBH III timeline entry linked to blog post, stats corrected (57 finalists, 91+ universities)

---

## 2026-04-10 — About Page Fact-Check (about.html)

1. **Timeline 2020-2023** — Changed "5 faculty" to "12 faculty". Source: Foundation Metrics FY23-24.
2. **Stats section** — Changed "27+ Faculty across 7 Departments" to "25+ Faculty Researchers" (consistent with homepage).
3. **Timeline 2025-2026** — Changed "42+ research outputs" to "30+ publications" (verified count). Changed "27+ faculty" to "25+ faculty".
4. **Mission text** — Removed promotional language ("pushes the frontiers", "secure critical internet infrastructure"). Simplified CHART description (removed false range pattern).
5. **Verified claims (no changes needed):** founding in 2020 (Phase 1 start), NeurIPS 2023 awards (1st + 4th place), 2023-2024 growth metrics (12→19 faculty, 76 students, 12 pubs), 10+ countries partnerships (11 verified), CNC routers (Mehta FX-1325V-ATC confirmed).

---

## 2026-04-06 — Homepage Fact-Check (index.html)

### Round 1 (Initial fact-check)
1. **BharatSim Spotlight description** — Fixed conflation. Old: "deployed to NACO for HIV prediction — covered by BBC, NDTV, and Nature India." New: Accurately describes H5N1 study and media coverage separately.
2. **OncoMark Spotlight journal name** — Fixed from "Nature Communications Biology" to "Communications Biology (Nature portfolio)."
3. **RedBrick Hacks III (Impact + News cards)** — Fixed: 60 → 57 finalists (individuals, not teams), added "91+ universities across 23 states", added "SDG-aligned" to tracks. Source: Q4 Report.
4. **Latest News section** — Updated 3 news items from pre-Q4 to latest Q4 events: WiCSCon 3.0 (Mar 21-22), ACM COMPUTE 2026 (Mar 21), ITiCSE papers accepted (Mar 2026).

### Round 2 (User feedback)
5. **Spotlight links fixed** — All 3 broken IDs corrected: `bharatsim-v2` → `bharatsim`, `oncomark` → `cancer-ascend`, `world-food-atlas` → `multimodal-food-computing`.
6. **OncoMark Spotlight pillar** — Changed from CHART to AI@Ashoka (matches projects.js `pillar: 'ai'`).
7. **Makerspace pillar card** — Removed "from table-top manufacturing to pedagogical tools", replaced with "powering interdisciplinary research and student projects."
8. **Oxford Fellowship card** — Removed "citing Mphasis-funded pilot data as foundational to her research." Replaced with "for her work on AI-driven pollen detection and biodiversity monitoring."
9. **Government Recognition card** — Added date (February 17, 2026).
10. **Dengue Drug Discovery card** — Replaced with IndiaMediaLens News Adjudication Monitor (no publication existed for Dengue; pressanalytics.in is a deployed system with real impact).
11. **Hero metrics** — Added 2 new stat cards: "25+ Faculty Researchers" and "40+ Collaborations". Grid updated from 4-col to 5-col.
12. **Pillar tags removed** from Latest News cards.
13. **Latest News cards** — Now link to individual blog post pages.

### Round 2 (Blog/Posts system)
14. **Blog system created** — `posts/` folder with individual HTML pages per news item. CSS in `src/css/post.css`.
15. **3 blog posts created:**
    - `posts/2026-03-wicscon-3.html` — WiCSCon 3.0 (Mar 21-22, 2026). Source: Q4 Report.
    - `posts/2026-03-acm-compute-2026.html` — ACM COMPUTE 2026 Workshop (Mar 21, 2026). Source: Q4 Report.
    - `posts/2026-03-iticse-papers-accepted.html` — ITiCSE papers accepted (Mar 2026). Source: Q4 Report.

### Key data verified
- **25+ Research Projects** — kept per user decision (actual count: 23)
- **30+ Publications** — verified
- **5 Research Pillars** — verified
- **25+ Faculty Researchers** — 25 names sourced from projects.js, people.js, Q4 Report
- **40+ Collaborations** — 41 unique institutions verified from projects.js + Q4 Report + Comprehensive Report
- **RedBrick Hacks III** — 430+ applicants, 91+ universities, 23 states, 57 finalists (individuals), 4 SDG-aligned tracks
- **OncoMark** — pillar: AI@Ashoka (not CHART or Makerspace), journal: Communications Biology
