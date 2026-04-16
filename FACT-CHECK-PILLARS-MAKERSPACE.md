# Fact-Check Report: Pillars Data & Makerspace Page

**Status: IN PROGRESS — Paused for session break**
**Date: February 28, 2026**
**Files Checked:**
- `/Users/raj/Desktop/projects/Workspace/Website/src/data/pillars.js`
- `/Users/raj/Desktop/projects/Workspace/Website/pages/makerspace.html`

**Verified Against:**
- Comprehensive Report: `Mphasis Annual Review - FY2025-26/Comprehensive Report/Mphasis Lab — FY2025-26 Comprehensive Progress Report.md`
- All 7 relevant fact sheets (CMT, Digital Makerspace, Pedagogical Experiments, Table Top Experiments, BharatSim, PQC, TNBC, Folk Computing, Multi-Modal Food Computing)

---

## DISCREPANCIES FOUND

### CRITICAL — Name Error

| # | Location | Claim on Website | Source Says | Severity | Action |
|---|---|---|---|---|---|
| 1 | `makerspace.html` line 276 | **"Correlated Magnetic Tweezers"** | **"Covalent Magnetic Tweezers"** — every source file, fact sheet, and the comprehensive report consistently uses "Covalent". The pillars.js data file also says "Covalent". | **CRITICAL** | Fix "Correlated" → "Covalent" in makerspace.html |

### HIGH — Factual Inaccuracies

| # | Location | Claim on Website | Source Says | Severity | Action |
|---|---|---|---|---|---|
| 2 | `pillars.js` line 106 (Makerspace description) | **"3 publications in Nature portfolio and major journal venues"** for CMT | CMT fact sheet lists **1 publication in Nature portfolio** (Communications Biology, DOI: 10.1038/s42003-025-08727-z) + 2 in other journals (Protein Science, Biochemistry). Comprehensive Report confirms the same: 1 Nature portfolio + 2 other journals. The phrase "3 publications in Nature portfolio" is misleading — only 1 is in Nature portfolio. | **HIGH** | Reword to "3 publications including one in Nature portfolio" or "1 Nature portfolio publication and 2 additional journal papers" |
| 3 | `makerspace.html` — Drone Fleet card (line 228) | Lists **"DJI Matrice 4T, Mavic 3E, and Mavic 4T"** | Digital Makerspace fact sheet says: DJI Matrice 4T (delivered, QC complete), DJI Mavic 3E (operational), DJI Mavic 4T (**approved only** — ~INR 6.7L + GST). The Mavic 4T purchase was approved but **no confirmation of delivery** found in any source. Comprehensive Report equipment table lists only "DJI Matrice 4T + DJI Mavic 3E." | **HIGH** | Either add "(on order)" qualifier for Mavic 4T, or remove it until delivery is confirmed. Flag for user input. |
| 4 | `pillars.js` — Makerspace description (line 106) | **"2,000 K-12 students engaged through outreach programs (672% of target)"** | Comprehensive Report says **"2,016+ school students"** reached through K-12 outreach (672% of 300 target). The "2,000+" in pillars.js is technically consistent as a rounded figure. **However**, the keyMetrics on line 109 says **"2,000+"** while the Comprehensive Report and makerspace.html both use **"2,016+"**. | **MEDIUM** | Consider using "2,016+" consistently, or keep "2,000+" as rounded. Minor issue. |
| 5 | `makerspace.html` — Table Top Experiments section (line 548) | **"All 3 interns placed at ANU (Australia), GIST (South Korea), University of Toronto"** | Table Top fact sheet says: Simar Randhawa → **ANU** (confirmed), Drishana Kundu → selected for Indian Academy of Sciences at NARL, **University of Toronto**, and **GIST South Korea** — **chose GIST**. The third intern (Bhavana) has **no documented placement**. The website says "All 3 interns placed" but only 2 have confirmed placements. Also, Drishana went to GIST, not University of Toronto. The wording implies 3 separate placements at 3 separate institutions, which is inaccurate. | **HIGH** | Rewrite: "Simar Randhawa placed at ANU (Australia), Drishana Kundu at GIST (South Korea)" — remove University of Toronto as a separate placement (it was one of Drishana's options, not where she went). Remove "All 3" unless Bhavana's placement is confirmed. |
| 6 | `pillars.js` — Cybersecurity description (line 88) | **"4 publications"** in keyMetrics | PQC fact sheet lists: (1) ACM ASIACCS 2025 — published, (2) Indocrypt 2024 — published, (3) SPACE 2023 — published (Best Paper Award), (4) IACR ePrint 2025/1770 — published on ePrint. That's 3 peer-reviewed publications + 1 ePrint preprint. Whether IACR ePrint counts as a "publication" is debatable — it's a preprint archive, not peer-reviewed. Also, #2 and #3 are from **prior fiscal years** (FY24 and FY23), not FY26. | **MEDIUM** | The "4 publications" is defensible if counting across all years and including ePrint. But for consistency, note that only 1 peer-reviewed publication is from FY26 (ACM ASIACCS 2025). Comprehensive Report confirms: "1 (ACM ASIACCS 2025)" for FY26 peer-reviewed + "3 technical reports (IACR ePrint + 2 internal)". Consider clarifying the metric label. |

### MEDIUM — Imprecise/Potentially Misleading Claims

| # | Location | Claim on Website | Source Says | Severity | Action |
|---|---|---|---|---|---|
| 7 | `pillars.js` — AI@Ashoka (line 11) | Description mentions **"Nature portfolio publication for cancer hallmark quantification"** | Confirmed: Communications Biology (Nature portfolio), DOI: 10.1038/s42003-025-08727-z for OncoMark. **Accurate.** | **OK** | No action needed |
| 8 | `pillars.js` — AI@Ashoka (line 11) | **"recognition by the Ministry of Electronics & IT in their India-AI Impact Summit Casebook"** | Confirmed: CS Pedagogy project selected for India-AI Impact Summit Casebook, MeitY, published at Bharat Mandapam, Feb 17, 2026. **Accurate.** | **OK** | No action needed |
| 9 | `pillars.js` — AI@Ashoka (line 11) | **"a patent filing for cancer diagnostics AI"** | Confirmed: Indian patent application 202511064233 filed for Cancer Ascend. **Accurate.** | **OK** | No action needed |
| 10 | `pillars.js` — AI@Ashoka (line 11) | **"a Schmidt AI for Science Fellowship at Oxford"** | Confirmed: Prof. Meghna Agarwala awarded 3-year Schmidt AI for Science Fellowship at Oxford, citing Mphasis-funded Pollen Project pilot data. **Accurate.** | **OK** | No action needed |
| 11 | `pillars.js` — AI@Ashoka keyMetrics (lines 12-17) | **"14 Projects", "8 Departments", "7+ Publications", "1 Patent Filed"** | Comprehensive Report confirms: 14 projects, 8 departments (CS, Biology, Chemistry, Physics, Psychology, Political Science, English, Economics — that's 8), 7+ publications (including Nature portfolio, ACM COMPUTE x3, EMNLP, NeurIPS + preprints), 1 patent filed. **All accurate.** | **OK** | No action needed |
| 12 | `pillars.js` — BharatSim (line 47) | Description says **"published in BMC Public Health"** for H5N1 paper | Confirmed: BMC Public Health, 25:3983 (2025). **Accurate.** | **OK** | No action needed |
| 13 | `pillars.js` — BharatSim (line 47) | **"coverage in over 20 international media outlets including BBC, CNBC-TV18, NDTV, Nature India, and the Sydney Morning Herald"** | Confirmed: Q3 report and Comprehensive Report list 20+ outlets including all named ones. **Accurate.** | **OK** | No action needed |
| 14 | `pillars.js` — BharatSim keyMetrics (lines 48-53) | **"20+ Media Outlets", "10+ Invited Talks", "1 National Deployment"** | Confirmed: 20+ media outlets (accurate), 10+ invited talks (fact sheet documents 10 individually; Comprehensive Report says "10+ in FY26" — accurate), 1 national deployment with NACO (confirmed — 1 predictive system complete, SOCH integration in progress). **All accurate.** | **OK** | No action needed |
| 15 | `pillars.js` — CHART description (line 66) | **"8-9 peer-reviewed publications in top venues including NeurIPS, ACM Multimedia, EMNLP, and IJCNLP-AACL"** | Comprehensive Report Section 4.3 says: "8-9 (NeurIPS, ACM MM x3, EMNLP, IJCNLP-AACL, plus 1 submitted, 1 in prep)". Let's count confirmed FY26 CHART publications: (1) NeurIPS/GenAI4Health — PRISM, (2-4) ACM Multimedia MMFood'25 — 3 papers, (5) EMNLP 2025 Findings, (6) IJCNLP-AACL JUST-NLP Workshop, (7) TNBC manuscript submitted. That's 6 published/accepted + 1 submitted + others in prep. The "8-9" may be inclusive of submitted manuscripts. | **MEDIUM** | The "8+" in keyMetrics is slightly generous if counting only peer-reviewed published papers (6 confirmed accepted/published). However, the Comprehensive Report itself uses "8-9" so the website is consistent with the Comprehensive Report. Flag for awareness but no change needed unless user wants stricter counting. |
| 16 | `pillars.js` — CHART keyMetrics (lines 68-72) | **"10,000+ Recipes in Database"** | Comprehensive Report Section 4.3 and MFC fact sheet confirm: "Food Composition Table was expanded to 10,000+ standardized recipes/ingredients — 2x the FY26 target of 5,000+." **Accurate.** | **OK** | No action needed |
| 17 | `pillars.js` — CHART keyMetrics (lines 68-72) | **"100 TNBC Patients Profiled"** | TNBC fact sheet confirms: "Completed profiling of 100 TNBC patients for immune infiltrates and 9 actionable molecular markers." **Accurate.** | **OK** | No action needed |
| 18 | `pillars.js` — CHART description (line 66) | **"the first International Workshop on Multimodal Food Computing (MMFood'25) at ACM Multimedia in Dublin"** | Confirmed in MFC fact sheet and Comprehensive Report. **Accurate.** | **OK** | No action needed |
| 19 | `pillars.js` — CHART description (line 66) | **"won the INFUSE Innovation Award"** | Confirmed: "Promising Innovation Award" at INFUSE Innovation Summit 2025 (NIN/ICMR, Hyderabad). The website says "INFUSE Innovation Award" while the full name is "Promising Innovation Award, INFUSE Innovation Summit 2025." | **LOW** | Minor — consider using full award name "INFUSE Promising Innovation Award" for precision |
| 20 | `pillars.js` — CHART description (line 66) | **"PRISM, the conversational AI system for abdominal pain diagnosis, was accepted at the NeurIPS 2025 GenAI4Health workshop"** | Confirmed in Folk Computing fact sheet. **Accurate.** | **OK** | No action needed |
| 21 | `pillars.js` — CHART description (line 66) | **"curated 4,800 breast cancer cases toward characterizing 5 TNBC molecular subtypes"** | TNBC fact sheet: "4,800 of 5,000 breast cancer cases completed." The 4,800 is of all breast cancer cases, not just TNBC. The 5 subtypes were characterized from the 100 TNBC patients specifically. The wording "4,800 breast cancer cases toward characterizing 5 TNBC molecular subtypes" could be misread as 4,800 TNBC patients — it's actually 4,800 total breast cancer cases curated (including non-TNBC). | **MEDIUM** | Consider rewording for clarity: "curated 4,800 breast cancer cases and characterized 100 TNBC patients across 5 molecular subtypes" |
| 22 | `pillars.js` — Cybersecurity description (line 88) | **"1 PhD completed"** in keyMetrics and description says **"a PhD thesis completed on post-quantum DNSSEC"** | PQC fact sheet: Aditya Rawat's PhD thesis was **submitted** to RDO on Nov 4, 2025, and is "currently with external examiners; degree expected within 1-2 months." The **defence is still pending** as of Feb 2026. So the PhD is not yet "completed" — the thesis is submitted but the degree has not been awarded. | **HIGH** | Change "1 PhD Completed" to "1 PhD Thesis Submitted" or "1 PhD Thesis Defended" (if defence has occurred by now — flag for user to confirm). The Comprehensive Report says "submitted Nov 4, 2025" and "defence pending." |
| 23 | `pillars.js` — Cybersecurity description (line 88) | **"a Best Paper Award at SPACE 2023"** | Confirmed: Best Paper Award at SPACE 2023 (Springer LNCS) for "Post-quantum DNSSEC over UDP via QNAME-Based Fragmentation." **Accurate**, though it's from FY23, not FY26. | **OK** | No action needed — FY23 award is appropriately listed as a project achievement |
| 24 | `pillars.js` — Cybersecurity description (line 88) | **"a publication at ACM ASIACCS 2025 (a top security conference)"** | Confirmed. **Accurate.** | **OK** | No action needed |
| 25 | `pillars.js` — Makerspace keyMetrics (line 111) | **"450+ Hackathon Applicants"** | This refers to RedBrick Hacks III only. Confirmed: 450+ applications from 91 universities. **Accurate for RBH III.** Note: makerspace.html uses "930+ Hackathon Applicants (All Editions)" — a different, aggregated number. | **OK** | No action needed — context is clear |

### MAKERSPACE.HTML SPECIFIC CHECKS

| # | Location | Claim on Website | Source Says | Severity | Action |
|---|---|---|---|---|---|
| 26 | `makerspace.html` hero (line 113) | **"4,500 sq ft fabrication facility"** | Digital Makerspace fact sheet: The new Makerspace facility was under construction with **Occupation Certificate pending as of December 2025**. The current operational Makerspace and the new facility dimensions are not explicitly stated as "4,500 sq ft" in any source file I found. Comprehensive Report says "New Makerspace Facility — Transition in progress (Occupation Certificate pending as of Dec 2025)." | **MEDIUM-HIGH** | The "4,500 sq ft" figure is not verifiable against any source document found. **Flag for user confirmation.** If this figure was provided verbally by the user or from a source not in the Source/ folder, it should be noted. |
| 27 | `makerspace.html` — Equipment list | **Trotec Speedy 400 Flexx** (line 171) | Comprehensive Report and fact sheet say **"Trotec Speedy 400"** — the "Flexx" designation is the dual-source variant (CO2 + Fiber). The 120W CO2 + 50W Fiber spec matches. | **LOW** | Technically more precise to include "Flexx" since it specifies the dual-source variant. No change needed — this is accurate detail. |
| 28 | `makerspace.html` — Equipment list | **Fabric & Textile Workstations — "Three industrial sewing machines"** (line 239) | Confirmed in Advisory Board Presentation: "Fabric Workstation (3 machines)." **Accurate.** | **OK** | No action needed |
| 29 | `makerspace.html` — Equipment list | **Wood Workshop — "staff with 15+ years of woodworking experience"** (line 250) | Digital Makerspace fact sheet: "Deepak Jangra — Lab Attendant (hired Oct/Nov 2025, 15+ years woodworking trade experience)." **Accurate.** | **OK** | No action needed |
| 30 | `makerspace.html` — Equipment list | **Mac Studio M4 Max workstations** (line 261) | Digital Makerspace fact sheet: "Mac Studio M4 Max — quotation stage" from InspireInfotech at INR 3,86,300. This was at **quotation stage**, not necessarily delivered. | **MEDIUM** | Flag for user — were Mac Studio M4 Max workstations actually delivered, or still in procurement? |
| 31 | `makerspace.html` — CMT section (line 277) | **"One of its kind in India"** | CMT fact sheet: "The CMT setup is described as unique in India, providing opportunities for research students to learn cutting-edge single-molecule instrumentation." Source: Q1 CMT.pdf, Deliverables section. **Accurate.** | **OK** | No action needed |
| 32 | `makerspace.html` — CMT publications section | Lists 3 publications: Communications Biology, Protein Science, Biochemistry | All 3 confirmed in CMT fact sheet with correct DOIs and journal references. **Accurate.** | **OK** | No action needed |
| 33 | `makerspace.html` — Maker-in-Residence section | **Ayush Tiwari (July 2025 – March 2026)** and **Ajad Ismail (August 2025 – March 2026)** | Digital Makerspace fact sheet confirms: Ayush Tiwari — Maker-in-Residence #1, SLAM Robot (Jul 2025–Mar 2026, INR 50,000/month); Ajad Ismail — Maker-in-Residence #2, Drosophila Thermal Maze (Aug 2025–Mar 2026, INR 50,000/month). **Accurate.** | **OK** | No action needed |
| 34 | `makerspace.html` — RedBrick Hacks winners invited | **"HarvesSink (greywater quality sensor) and Tap-Box (refreshable braille display) — invited for summer Maker-in-Residence fellowships starting June 2026"** | Comprehensive Report: "Two winning teams (HarvesSink, Tap-Box) invited for Maker-in-Residence follow-up at the Makerspace." **Accurate**, though "starting June 2026" is not explicitly stated in sources — could be user-provided information. | **LOW** | Minor — "June 2026" start date not confirmed in source. Flag for user if needed. |
| 35 | `makerspace.html` — K-12 Outreach | **"2,016+"** and **"672% of annual target"** | Comprehensive Report: "2,016+ school students reached (672% of 300 target)." **Accurate.** | **OK** | No action needed |
| 36 | `makerspace.html` — Partnerships | **"Param Foundation"** (line 706) | Comprehensive Report says **"Param Innovation"** — and describes it as "MoU signed September 24, 2025." The website says "Param Foundation" which appears to be a different name. | **MEDIUM** | Verify: Is it "Param Foundation" or "Param Innovation"? The Comprehensive Report and fact sheet consistently use "Param Innovation." Fix if incorrect. |
| 37 | `makerspace.html` — Partnerships | **TinkerHub Foundation, Maker Bhavan Foundation, Stanford University** | All confirmed in Comprehensive Report Section 3.2. TinkerHub Foundation — student maker community. Maker Bhavan Foundation — ecosystem partner. Stanford — ShistoDx team collaborating with Prof. Manu Prakash. Note: Comprehensive Report also mentions **Passionfruit Labs** as an industry mentorship partner, which is not listed on the makerspace page. | **LOW** | Consider adding Passionfruit Labs if desired. Not a discrepancy, just an omission. |
| 38 | `makerspace.html` — Drosophila Thermal Maze | **"Only 2–3 labs globally have built this apparatus"** (line 392) | Digital Makerspace fact sheet: "Drosophila thermal maze — only 2-3 labs globally." **Accurate.** | **OK** | No action needed |
| 39 | `makerspace.html` — Dots: Tactile Dot Grid | **"25% the cost of commercial alternatives. Presented at HCII 2025, Gothenburg, Sweden."** (line 416) | Comprehensive Report lists "Dots: Refreshable Tactile Dot Grid (poster)" at HCII 2025, Gothenburg, Sweden. The "25% cost" claim is not found in any source file reviewed. | **MEDIUM** | The "25% the cost" claim needs a source citation. Flag for user to confirm or remove. |
| 40 | `makerspace.html` — Events list | **"Indian Academic Makerspaces Summit, IIT Gandhinagar. 160+ participants."** (line 660) | Not found in Comprehensive Report or Digital Makerspace fact sheet. This event may be sourced from the Q3 Data Dump document referenced in the fact sheet. Cannot independently verify attendance figure. | **LOW** | Flag for user — source for "160+ participants" at IIT Gandhinagar? |

---

## SUMMARY OF REQUIRED FIXES

### Must Fix (Critical/High):
1. **makerspace.html line 276**: "Correlated Magnetic Tweezers" → "Covalent Magnetic Tweezers"
2. **pillars.js line 106**: "3 publications in Nature portfolio" → "3 publications including one in Nature portfolio" (or similar rewording)
3. **makerspace.html line 228**: Mavic 4T listed as current equipment — it was only approved, not confirmed delivered. Add qualifier or remove.
4. **makerspace.html line 548**: "All 3 interns placed at ANU, GIST, University of Toronto" — only 2 confirmed placements; U of Toronto was an option Drishana declined. Rewrite.
5. **pillars.js line 92**: "1 PhD Completed" → "1 PhD Thesis Submitted" (defence still pending per sources)

### Should Fix (Medium):
6. **pillars.js line 66 (CHART)**: Clarify 4,800 breast cancer cases vs 100 TNBC patients wording
7. **makerspace.html hero**: "4,500 sq ft" — not verifiable in sources; flag for user confirmation
8. **makerspace.html line 706**: "Param Foundation" should likely be "Param Innovation" per sources
9. **makerspace.html line 261**: Mac Studio M4 Max — was at quotation stage in sources; confirm delivery
10. **makerspace.html line 416**: "25% the cost" for Dots project — no source found

### Optional (Low):
11. INFUSE award — consider full name "Promising Innovation Award"
12. Passionfruit Labs partnership — not listed on makerspace page (omission, not error)
13. "June 2026" start for RedBrick winners' residency — not in sources
14. IIT Gandhinagar summit "160+ participants" — source not found in reviewed files

---

## VERIFIED AS ACCURATE (No Issues)

### AI@Ashoka Pillar:
- 14 projects across 8 departments ✅
- 7+ publications ✅
- 1 patent filed ✅
- Nature portfolio publication (OncoMark/Cancer Ascend) ✅
- MeitY India-AI Impact Summit Casebook selection ✅
- Schmidt AI for Science Fellowship at Oxford ✅
- All research themes listed ✅
- All 14 project slugs match known projects ✅

### BharatSim Pillar:
- 20+ media outlets ✅
- 10+ invited talks ✅
- 1 national deployment (NACO) ✅
- BMC Public Health publication ✅
- Named media outlets (BBC, CNBC-TV18, NDTV, Nature India, Sydney Morning Herald) ✅
- Description of H5N1, mpox, HIV/AIDS, dengue modelling ✅
- Wellcome Trust, WHO-SEARO, IIT Bombay mentions ✅

### CHART Pillar:
- 3 projects ✅
- 10,000+ recipes in database ✅
- 100 TNBC patients profiled ✅
- MMFood'25 at ACM Multimedia ✅
- PRISM at NeurIPS 2025 GenAI4Health ✅
- NeurIPS, ACM Multimedia, EMNLP, IJCNLP-AACL venue mentions ✅

### Cybersecurity Pillar:
- 1 project ✅
- 1 Best Paper Award (SPACE 2023) ✅
- ACM ASIACCS 2025 publication ✅
- IACR ePrint formal proof ✅
- SL-DNSSEC description ✅
- TCP hijacking research mention ✅

### Makerspace Pillar:
- 4 core projects ✅
- 450+ hackathon applicants (RBH III) ✅
- K-12 outreach numbers (2,016+, 672%) ✅
- Equipment list (Trotec, CNC, SLS/SLA, Jyoti DX60) ✅
- CMT as "unique in India" ✅
- Maker-in-Residence details (Ayush Tiwari, Ajad Ismail) ✅
- RedBrick Hacks III stats (91 universities, 60 finalists) ✅
- Cross-pillar support (Pollen, Fire Mapping, AIM-Flow) ✅
- Student placements from Table Top (ANU, GIST — 2 of 3 confirmed) ✅
- Pedagogical Experiments completion ✅

---

## FILES READ DURING THIS FACT-CHECK

1. `/Users/raj/Desktop/projects/Workspace/Website/src/data/pillars.js` — Full file
2. `/Users/raj/Desktop/projects/Workspace/Website/pages/makerspace.html` — Full file
3. `/Users/raj/Desktop/projects/Workspace/Mphasis Annual Review - FY2025-26/Comprehensive Report/Mphasis Lab — FY2025-26 Comprehensive Progress Report.md` — Full file (all sections through Appendices)
4. `/Users/raj/Desktop/projects/Workspace/Mphasis Annual Review - FY2025-26/Project Fact Sheets/Makerspace/CMT — Debayan Gupta.md` — Full file
5. `/Users/raj/Desktop/projects/Workspace/Mphasis Annual Review - FY2025-26/Project Fact Sheets/Makerspace/Digital Makerspace — Deepraj Pandey.md` — Full file
6. `/Users/raj/Desktop/projects/Workspace/Mphasis Annual Review - FY2025-26/Project Fact Sheets/Makerspace/Pedagogical Experiments — Pramoda Kumar.md` — Full file
7. `/Users/raj/Desktop/projects/Workspace/Mphasis Annual Review - FY2025-26/Project Fact Sheets/Makerspace/Table Top Experiments — Pramoda Kumar.md` — Full file
8. `/Users/raj/Desktop/projects/Workspace/Mphasis Annual Review - FY2025-26/Project Fact Sheets/BharatSim/BharatSim — Gautam Menon.md` — Full file
9. `/Users/raj/Desktop/projects/Workspace/Mphasis Annual Review - FY2025-26/Project Fact Sheets/Cybersecurity/PQC — Mahavir Jhawar.md` — Full file
10. `/Users/raj/Desktop/projects/Workspace/Mphasis Annual Review - FY2025-26/Project Fact Sheets/CHART/TNBC — L.S. Shashidhara.md` — Full file
11. `/Users/raj/Desktop/projects/Workspace/Mphasis Annual Review - FY2025-26/Project Fact Sheets/CHART/Multi-Modal Food Computing — Lipika Dey.md` — Full file
12. `/Users/raj/Desktop/projects/Workspace/Mphasis Annual Review - FY2025-26/Project Fact Sheets/CHART/Folk Computing — Rintu Kutum.md` — Full file

## WORK REMAINING

- [ ] Apply fixes for the 5 critical/high issues
- [ ] Get user confirmation on flagged items (4,500 sq ft, Mavic 4T delivery, Mac Studio delivery, PhD defence status, Dots cost claim)
- [ ] Check Makerspace "4 publications" claim in detail — which 4? (CMT has 3 FY26; Comprehensive Report lists 4 for Makerspace pillar: Communications Biology, Protein Science, Biochemistry, Royal Society B/Spiti Valley, HCII 2025 — that's actually 5)
- [ ] Verify the "Param Foundation" vs "Param Innovation" naming with user
