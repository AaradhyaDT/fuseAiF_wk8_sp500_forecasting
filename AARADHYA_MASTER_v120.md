# AARADHYA DEV TAMRAKAR — Master Profile v120

*Last updated: June 26, 2026 — v120: **Patch System + Fellowship Priority Trigger added.** (1) **Patch-based update system documented** — large-context AI (Gemini/Copilot) scans a repo and writes a structured documentary `PATCH_*.md` capturing what was done, what was built, what was learned, mistakes, and open items; patches are brought back to Claude alongside master profile for merge into new version; patch format also serves as a speed-replay log for reviewing a whole week's work in 2–3 minutes; patch template + Gemini extraction prompt added as §17; (2) **Fellowship Priority Trigger added to Session Loading Instructions** — repo naming convention (`fuseAiF_*`) auto-activates fellowship mode; portfolio, CV, and LinkedIn updates also trigger it; trigger instructs Claude to load fellowship context first, apply 12-Factor checklist gate, check week progression, and default to patch-aware session workflow; (3) No content altered elsewhere — all other sections unchanged from v119.*

*Previous: v119: Temporal sync pass + site static-fallback fixes. **Today:** Project Part A (Jun 26) — IV/I exam period at its final boundary; outcome not yet logged. Phase map updated to reflect exams complete. **Site fixes applied** (`aaradhyadtmr_github_io_v12.zip`): (1) **Static fallback for `live-focus`** — v118 session described fixing this but the v11 zip was packaged before those changes landed; corrected from stale "PrakopNet Major Project (proposal July 2) · Fuse AI Fellowship complete" to accurate "PrakopNet proposal due Jul 2 · Fuse AI Fellow — Wk 8/24 ongoing"; (2) **Static fallback for `live-fellowship`** — corrected from "SQL Associate next" to "SQL Associate underway"; (3) **JS template for `live-fellowship`** — updated to include "SQL Associate underway" detail (was dropping it once JS ran); (4) **`sitemap.xml`** — dates updated 2026-06-25 → 2026-06-26. Fellowship status: Wk 8/24, Jun 22–Jun 28, ongoing. PrakopNet proposal deadline: July 2 (6 days). **Pending (unchanged from v118):** CV PDF still says "Weeks 1–7 complete" — needs manual .docx update; Algoverse outcome still unresolved; GitHub Pages live/push status still unconfirmed.*

*Previous: v118: Cross-document consistency audit — portfolio site bug fixes + master profile deep temporal/structural check. **Portfolio site fixes** (`aaradhyadtmr_github_io_v11.zip`): (1) **Quick-nav numbering bug fixed** — "Where to look next" card index labels (`P — NN`) were frozen to each page's position in a fixed master order, so excluding the current page left a gap (e.g. `about.html` jumped 01→02→03→05 with no 04); now renumbered sequentially per page on all 6 HTML files; (2) **Stale Fellowship-complete claim fixed** — `index.html` status card's no-JS static fallback said "Fuse AI Fellowship complete" and "PrakopNet Major Project," contradicting the v117 live engine's correct "Wk 8/24 ongoing" / "proposal due Jul 2" computation for today's date; both the static fallback and the `live-fellowship` JS template corrected, "SQL Associate underway" detail preserved; (3) Verified (no bug): cert file wiring (19 buttons / 16 items: 13 single + 1 six-cert DataCamp bundle + 2 intentionally cert-less), `IEEE_KEC_Volunteering_Vice_Secretary` cert (wired via `experience.html`, not orphaned), BEI semester switch logic, og-image dimensions, EmailJS/Formspree config, GA4 single-load, all internal hrefs. **Master profile fixes** (this file): (4) **Fellowship duration contradiction resolved** — "Common cases" reference table (§Session Loading Instructions) and the "Actual Situation & Path" narrative both still said "7-week structure... ends mid-2026," contradicting the authoritative 24-week/Oct 18 2026 end date established at v117 elsewhere in the same doc; both corrected to 24-week/Wk 8/24 ongoing; (5) **Stale Netlify + Decap CMS architecture description removed** — two leftover paragraphs (in "Actual Situation" and in the Portfolio Website section) still described the pre-cancellation `/content/*.json` + Decap CMS + Netlify architecture, directly contradicting the v111 cancellation decision and the v113 "staying on GitHub Pages" status box; replaced with accurate static multipage description; (6) **Exam schedule "← TODAY" marker removed** — was anchored to Jun 12, 13 days stale; Jun 12/15/19 exam outcomes flagged "not logged" rather than silently assumed passed; (7) **Algoverse AI Research application flagged** — deadline (May 24) passed with no outcome ever logged; cohort (Jun 7–Aug 30) is currently in progress, meaning if accepted this is an unreconciled concurrent full-time commitment — flagged in both the table entry and narrative mention for follow-up, not guessed at; (8) **Project numbering/ordering bug fixed** — items 12–15 under §Projects were in document order 14,15,12,13 (inserted out of sequence across sessions); reordered to 11→12→13→14→15 matching chronology, headers renumbered, no content altered; (9) **Stale counts corrected** — `experience.html` timeline cited as "7-item" in Build progress table, actually 8 (Makerspace Ambassador added v116, count never bumped); achievements cert count cited as "13 wired, 3 no file," actually 19 buttons/16 items/2 no-file as of today (NepaTronix Drone cert added since v114, no longer cert-less). **Flagged, not fixed — needs your input:** CV PDF (`AARADHYA_DEV_TAMRAKAR_CV.pdf`) still says "Weeks 1–7 complete"; `.docx` source not in this upload, so it can't be regenerated here — needs manual update from source. GitHub Pages live/not-live status could not be independently verified (no network access to confirm); local dev-server screenshots (port 5500) are consistent with "not yet pushed" but not conclusive — confirm directly.*

*Previous: v117: Portfolio live-date engine added + Fusemachines 24-week completion logic. Key changes: (1) **Live date engine in `script.js`** — `computeLiveDates()` and `applyLiveDates()` added to shared script; runs at boot on every page; exposes `window.LIVE` object with `fuseWeek`, `fuseLabel`, `fuseStatus`, `semLabel`, `semFull`, `heroTag`, `subjects`; (2) **Fuse AI Fellowship auto-updating week display** — anchor May 4 2026 (Wk1 Mon), Mon–Sun cadence, flips every Monday 00:00 local; label format: `Fuse AI Fellow — Wk N/24 (Mon Date–Sun Date) ongoing`; total duration = **24 weeks (6 months)**, ends Oct 18 2026 (Sun); from Oct 19 2026 (Mon) 00:00 label switches permanently to `Fuse AI Fellowship — Completed (May–Oct 2026, 24 wks)`; (3) **BEI semester auto-switch** — IV/I until Sep 1 2026 00:00, then IV/II; hero-tag, edu-meta, stat labels, subject tags all update automatically; IV/II subjects: Telecommunications, Professional Practice, Energy/Environment/Society, Information Systems, Elective II (EX 765), Elective III (EX 785), Project Part B — PrakopNet; (4) **Pages wired**: `index.html` (hero-tag, Focus status item, Fellowship status item, stats strip semester label), `about.html` (year stat, edu-meta paragraph, coursework title, subject tags), `experience.html` (Fuse AI Fellow timeline year column); (5) **Semester boundary rule hardcoded**: IV/II only from Sep 1 2026 — completing IV/I exams does not trigger the switch; (6) **PrakopNet proposal deadline** (July 2 2026) wired into Focus item — shows "PrakopNet proposal due Jul 2" before deadline, switches to "PrakopNet Major Project" after; (7) **GA4 double-load bug fixed** (carried from v116 — inline GA4 blocks removed from all 6 HTML pages; script.js `loadGA4()` is sole handler); (8) Makerspace Ambassador added to `experience.html` timeline; JavaScript/React added to `about.html` skills; Fuse fellowship year in experience.html now live-computed. Deliverable: `aaradhyadtmr_github_io_v9.zip` (files changed: `assets/js/script.js`, `index.html`, `about.html`, `experience.html`, + all pages from v116 fixes).*

*Previous: v116: Portfolio site session — GA4 double-load bug fixed (script.js already had loadGA4() in boot; last session added duplicate inline blocks to all 6 pages — removed); Makerspace Ambassador entry added to experience.html; JavaScript/React added to about.html skills; Fuse fellowship status updated in experience.html; status card Focus/Stack updated; "Active Fellowships" stat → "Fellowships & Grants"; sitemap dates → 2026-06-25. BEI IV/I confirmed correct (IV/II change reverted after user correction). Temporal Status Verification AUTO-TRIGGER added to Session Loading Instructions.*

*Last updated: June 25, 2026 — v116: Portfolio site session — two-pass optimization and content refresh on `Aaradhya-Dev-Tamrakar_github_io-updated.zip` (previously output of last session). Key changes: (1) **GA4 double-load bug fixed** — script.js already contained `loadGA4()` in its boot sequence; last session added a duplicate inline GA4 loader block to all 6 HTML pages, causing double config firing; inline blocks removed from all 6 pages (script.js handles GA4 exclusively now); (2) BEI IV/I confirmed correct — semester designation unchanged; (4) **JavaScript / React added to about.html skills** — Programming Languages group, 2/3 proficiency dots (missing from skills since v113); (5) **Fuse AI Fellow fellowship** — updated to completed status in `experience.html` (year changed from "2026 — Present" to "2026"); bio in `about.html` changed from "I'm currently a Fuse AI Fellow" to "I'm a Fuse AI Fellow"; (6) **Makerspace Ambassador added to experience.html** — new timeline entry (KEC Maker's Space · June 2026–Present); (7) **Status card** (`index.html` hero) — Focus item updated from "Fuse AI Fellowship — Wks 1–7 complete · PrakopNet Major Project" to "PrakopNet Major Project (proposal July 2) · Fuse AI Fellowship complete"; Stack item now includes JavaScript/React; (8) **"Active Fellowships" stat** changed to "Fellowships & Grants" in both `index.html` and `about.html` (Fuse AI is complete, not active); (9) **`sitemap.xml` dates** updated from 2026-06-22 → 2026-06-25. Deliverable: `aaradhyadtmr_github_io_v9.zip` (7 files changed: `index.html`, `about.html`, `experience.html`, `projects.html`, `achievements.html`, `contact.html`, `sitemap.xml`).*

*Last updated: June 24, 2026 — v115: PrakopNet §8 updated — full session integration from June 24, 2026 holiday alignment prep session. Key changes: (1) Proposal deadline confirmed July 2, 2026; (2) Supervisors not yet assigned (group formation different from last year — pending 8th semester); (3) OOSE framing added (Factory pattern for nodes, Observer pattern for gateway→alerts); (4) WP numbering formalised (WP 1.0–4.0); (5) Animal behavior precursors (Umesh/HPCNepal) confirmed de-scoped → Chapter 6 Future Work only; (6) ICIMOD RIMS confirmed as primary data source alongside DHM; (7) Module C scope conflict documented (Phase 5 reinstated; Gemini Phase 6 deleted — decision deferred to June 24 meeting); (8) HazardScore equation refined to `w_f·(ΔD/Δt) + w_l·(Δθ/Δt)` with named variables; (9) Sonia LaTeX scope clarified — proposal Overleaf layout only, not ongoing thesis; (10) PrakopNet_MASTER_v0_20260624.md generated as new operative project truth; (11) Key documents updated — ChronologicalMerge v4, TEAM_PROFILE_SYSTEM v17, gemini_phase_6_.md absorbed. Star vs mesh topology still unresolved — Rupesh to own call before August.*

*Previous: v114: CV updated to `AARADHYA_DEV_TAMRAKAR_CV_June22_2026.docx` — Profile paragraph updated ("Weeks 1–7 complete"), Last Updated date updated to June 22, 2026. `achievements.html` updated: all 13 certificates with matching files wired to inline lightbox modal (frosted-glass backdrop, slide+scale entrance, PDF iframe + PNG img rendering, ESC/backdrop/✕ close, Download + Open-in-new-tab actions, keyboard focus trap); 3 items without certificate files left without button (IEEE Conference Leadership, NepaTronix Drone, Git & GitHub). `IEEE_KEC_Volunteering_Vice_Secretary_2025_2026.png` exists in `/certificates/` but belongs to `experience.html` — not yet wired.*

*Previous: v113: Portfolio multipage migration **fully complete** (all 6 rounds shipped in same session as v112). Round 3: `projects.html` (full projects grid — GCSBR, Alpha, Edge AI, Nexus, PrakopNet, Fuse Wk3–Wk7, Antenna, Custom Processor; card hover reveal, tag system, GitHub/demo links). Round 4: `experience.html` (7-item timeline — Fuse AI Fellow Wk1–Wk7, IEEE VC, NSSR DataCamp, EPC Event Manager, IEEE VS, EPC Co-Host, EPC Resource Manager; 3-col grid layout). Round 5: `about.html` (bio 3 paragraphs, `<picture>` WebP photo + ring animation, 4-stat strip, 3-group skills grid, education card with coursework tags, tools row, CV download). Round 6: `contact.html` (3 contact links with orbit-ring hover, EmailJS form — service `service_ndgwufl` / template `template_537qrr1` — Formspree `mrejgjyd` fallback, mailto last resort). Post-rounds: `sitemap.xml` updated with all 5 page URLs, `README.md` rewritten for multipage architecture. OG image fix also completed in same session: `og-image.jpg` generated at 1200×630 (dark brand background, subject right-aligned), all 5 pages updated to reference it with correct dimensions, JSON-LD Person.image left as `photo.png`. Full deploy package: `aaradhyadtmr_github_io_v7.zip` (22 files) — ready to push to GitHub Pages. **NOT YET LIVE** — zip built and verified but not yet committed/pushed to repo. Deliverables: all 5 HTML pages + `assets/css/style.css` + `assets/js/script.js` + `sitemap.xml` + `README.md` + `og-image.jpg` (in v7 zip).*

*Previous: v111: Portfolio multipage migration decided — Netlify + Decap CMS cancelled, staying on GitHub Pages. Single-file `index.html` converting to 5-page static site (`index`, `projects`, `experience`, `about`, `contact`). Full GitHub Copilot (Raptor mini) build plan + ranked pattern reference added to Portfolio Website §. Portfolio hosting quick-ref updated. Week 7 Clustering Assignment portfolio trigger updated (Decap CMS path removed, points to `projects.html` in new multipage structure). KEC Makerspace site audited as architecture reference (June 22, 2026) — zip will not be re-uploaded; all patterns documented in build plan.*

*Previous: v110: Instructor feedback note updated — router/subfolder feedback linked to same session as 12-Factor standard (§16, v99); both are the same code-quality push.

*Previous: v109: Instructor feedback logged in Fellowship Dev Standards — declutter into subfolders + separate FastAPI routers per domain (exact week unconfirmed, Wk 2/3/4 API project). Apply-forward rule added: all new FastAPI projects must use APIRouter per domain from day one.*

*Previous: v108: Effort Level & Thinking Mode optimal usage guide added to Claude Pro ROI Assessment section — task-mapped table (effort/thinking combos), token cost reality, and the default rule (High/OFF → Max/ON only when stuck or making irreversible decisions).*

*Previous: v107: eSewa QA Intern screening result logged under Screened Opportunities — written exam passed, not selected due to full-time conflict; CV forwarded to F1Soft sister organizations. Claude Pro ROI section added to Banking & Subscriptions (Planned Subscriptions table expanded, ROI Assessment table added, primary payment via trusted contact's dollar card). Claude Pro ROI auto-trigger instruction added to Session Loading Instructions.*

*Previous: v106: Claude Pro ROI section added to Banking & Subscriptions. GitHub Education Pack application logged. Planned Subscriptions table expanded with status column. Primary payment method: using a trusted contact's dollar card; SBL E-com Card and GitHub Edu Pack as fallbacks.*

*Previous: v105: PageSpeed Insights live-verification session on `aaradhyadtmr.github.io`, following up on v104's mobile FCP/LCP fix. Live PSI test post-v104 deploy: desktop 99, mobile 95 → LCP 2.7s (FCP 1.7s) — confirmed the v104 fix worked, but PSI flagged two new findings not previously caught: (1) **forced reflow** in both canvas resize handlers (`pcb-canvas`/PCB-trace background, `bg-canvas`/SignalWaveBackground) — `this.W = this.canvas.width = window.innerWidth; this.H = this.canvas.height = window.innerHeight;` wrote to `canvas.width` then read `window.innerHeight` on the next line, forcing a synchronous layout between write and read; fixed by reading both viewport values into local consts before any canvas write; (2) **mobile LCP candidate was the nav-logo ("ADT."), not the hero heading** — `.hero-name` (the real LCP element) had `opacity:0` + a `fadeUp 0.9s 0.35s` entrance animation, so Chrome's LCP detector skipped it as invisible-at-first-paint and picked the always-visible nav logo instead. **Two incorrect fix attempts were made and reverted before landing on the verified-correct one** — logged here so this isn't re-attempted: (a) compressing all four hero fade-up delays into a ~0.66s window (treating it as a "make the invisible window shorter" problem) caused 95→78 mobile in PSI, reverted; (b) removing `opacity`/`animation` from `.hero-name` only, isolated to that one element — ALSO measured 78 mobile on the very next run, prompting a full revert back to byte-identical v104 hero CSS (timing unchanged: tag 0.2s, name 0.35s, desc 0.5s, actions 0.65s, right-card 0.7s) — at which point a **second PSI run on the unchanged-from-v104 hero block also showed 80 mobile**, with Element render delay spiking from 280ms to 1,280ms despite zero code difference, confirming the 78–80 readings were **PSI lab-run noise/variance** (shared GitHub Pages infra + Slow-4G throttling simulation), not a real regression. **User re-ran PSI and got consistent 92 mobile / 99 desktop** — confirms the forced-reflow fix is net-positive and the hero-animation/LCP-detector issue, while real, was not solved by either of the two attempted edits; current live `index.html` hero CSS is identical to v104 (no opacity/animation changes survived), only the two canvas resize reflow fixes are new on top of v104. **Lesson logged**: do not re-attempt hero-entrance-animation timing changes to chase the LCP-detector/nav-logo issue without a real Chrome DevTools Performance trace (not just a PSI PDF) to confirm which element is actually being measured frame-by-frame — two plausible-sounding CSS-only theories were both wrong, and PSI single-run mobile scores can swing ±15-20 points run-to-run on unchanged code, so single-run deltas should not be read as causal without a re-test first. Deliverable: `index.html` (canvas resize reflow fix only, retained from this session; hero CSS reverted to v104 state).*

*Previous: v104: Portfolio mobile performance fix session on `aaradhyadtmr.github.io`. Root cause of stuck ~3s mobile FCP/LCP found: hero text (the LCP element) was empty in HTML, only filled by a ~90KB inline `<script>` at the bottom of a 161KB single-file page — nothing could paint until the whole document downloaded and ran. Fixed: (1) hero text/tagline/status-card items converted to static HTML (paint on CSS-ready, zero JS dependency; `DATA`-driven script still re-renders them as source of truth — manual sync note added: editing `DATA.tagline/headline/description/status` requires updating static hero markup too); (2) `<link rel="preload" as="image" href="photo.png">` removed — photo lives in About, not hero, so it was stealing mobile bandwidth from actual LCP-gating resources (this **reverses** the v66 decision logged below to preload photo.png — that earlier choice is now superseded); (3) `img.loading` fixed from `"eager"` to `"lazy"` on photo (now matches README claim); (4) photo optimized: 1000×1000 PNG (222KB) → 720×960 3:4 crop, WebP primary (60KB) + quantized PNG fallback (81KB) via `<picture>`, transparency preserved, ~73% smaller; (5) forced-reflow fix — `img.offsetWidth/offsetHeight` geometry read deferred to next frame (was forcing synchronous layout during image load); (6) Google Fonts request trimmed to only weights/styles actually used (preload + stylesheet + noscript all updated consistently); (7) inline CSS minified — file dropped 161KB → 133KB, content strings/animations/`clamp()` values verified intact; (8) EmailJS lazy-loaded, submit handler ensures it's loaded before send. Fonts/CSS loading strategy (preconnect, font-display swap, size-adjust fallbacks) was already well-built — not touched. Separately: user surfaced a Google AI Mode claim that GA4 was "missing the core script file request and measurement initialization tag" — **verified false**. `gtag('js', new Date())`, `gtag('config', 'G-P38642CDGB')`, and the `googletagmanager.com` script tag all exist (lines ~1927–1931), correctly deferred to post-load instead of `<head>` (intentional FCP-safe pattern per v66). AI Mode only inspected the `<head>` dataLayer stub and missed the deferred block further down — false positive, no action taken. Deliverables: `index.html` (updated), `photo.webp`, `photo.png` (optimized).*

*Previous: v103: Portfolio SEO hardening session on `aaradhyadtmr.github.io` (current live state: plain GitHub Pages, single-file vanilla JS — Netlify + Decap CMS is a **planned future migration, not yet executed**; user is also considering GitHub Projects for a multi-page site as an alternative). `index.html` already had strong on-page SEO (title/meta description, OG + Twitter cards, canonical, JSON-LD Person schema, single H1, proper heading hierarchy). Added the two missing pieces: `robots.txt` (Allow: / + sitemap reference) and `sitemap.xml`, both pushed to repo root and confirmed live via direct URL fetch. Created and verified a Google Search Console property (URL prefix, HTML-file verification method — `google3e772e11a3eb8313.html` uploaded to repo root, ownership verified). Submitted `sitemap.xml` via Search Console Sitemaps report. Settings → Crawling showed "No robots.txt file" / "No data available yet" with Open Report buttons greyed out immediately post-verification — confirmed normal for a brand-new property (no crawl cycle yet), not a bug; live file fetch confirmed robots.txt correct. Flagged but unresolved: `og:image`/`twitter:image`/JSON-LD `image` point to `photo.png` at 400×500, which is undersized/wrong-aspect for OG previews (ideal 1200×630) — fix not yet applied. Also flagged: no `theme-color` meta tag; JSON-LD could add `knowsAbout`/richer `worksFor`. Deliverables: `robots.txt`, `sitemap.xml` (both in repo).*

*Previous: v102: KEC Makerspace website (`KEC-innovation/makerspace-main`) work logged as the active Makerspace Ambassador web-dev deliverable. Established a Claude-as-orchestrator + GitHub Copilot Pro "Raptor mini" (preview model) execution workflow — Claude audits the live repo and writes scoped copy-paste prompts; Raptor mini executes them in VS Code Agent/Edit mode. Four rounds shipped same-day: (1) site-wide bug fixes — malformed `<img loading>` attribute bug (48 instances/17 files, root-caused to a regex bug in `scripts/optimize_site.py` + `fix_site_optimization.py`, now fixed plus a new `repair_img_tags.py`), unified opening hours across 3 stale sources, 3D Scanner badge/alt-text fix, SOP buttons wired to `docs/*.md` (stub content, not final), 2× Bambu Lab A1 printer card added, hero photo swapped to a real interior shot; (2) follow-up audit found SOP docs are still stubs, the new Bambu A1 card's SOP button mislinks to `get-started.html`, `.tag-required/.tag-free/.tag-soon` CSS is duplicated/inconsistent between `style.css` and an inline block in `offerings.html`, and a stale Apr-26 event is still sitting in "Upcoming"; (3) font audit root-caused site-wide faux-bold headings — Changa One / Gravitas One are loaded at weight 400 only (no real bold cut exists on Google Fonts) but `h1–h4` default to browser-bold and 7 elements force 700/800 on top, causing browser-synthesized distortion (Syne is fine, loaded at real 600/700/800; Rammetto One is loaded on all 17 pages but used nowhere — dead weight + an orphan CSS class; `--text-faint` also fails WCAG AA contrast in both themes); (4) navbar animation proposals (sliding underline, hamburger→X morph, mobile-nav slide transition, theme-toggle icon cross-fade, scroll-elevation shadow, logo hover lift) wrapped in a `prefers-reduced-motion` guard out of respect for a prior in-repo decision to strip animations, plus a found bug where the desktop active-nav-link color (`--accent`) doesn't match the mobile one (`--accent2`). Pending real SOP content and Thursday-workshop details before the event-system tasks can be finished.*

*Previous: v101: Dual-boot/partition/BitLocker setup documented (Ubuntu 26.04 LTS "Resolute Raccoon", Secure Boot ON, Fast Startup OFF; 1TB NVMe layout: C: 701.82GB / D: 150GB BitLocker / Ubuntu root 92.2GB / swap 7.8GB). Both Windows volumes BitLocker-encrypted via TPM+Secure Boot Device Encryption — manual `cryptsetup bitlkOpen` unlock flow documented (GUI paste unreliable). Recovery keys live on Microsoft Account + SD card backup, matched by Key ID (full key digits deliberately not stored in this doc). Time-sync dual-boot clock drift fixed via `timedatectl set-local-rtc 1`. Intel Arc iGPU confirmed working natively (Mesa, in-kernel) with VA-API hardware video decode verified (`intel-opencl-icd intel-media-va-driver` — note renamed package on 26.04, needs universe/multiverse repos). D: drive automount blocked by encryption; keyfile-based auto-unlock not yet implemented.*

*Previous: v100: Acer Swift Go 16 fan issue diagnosed and resolved. Root cause: GNOME Power Mode set to "Power Saver" was capping load below the EC's fan-trigger threshold — not a driver/firmware/EC fault. `acpi-fan`, `acer_wmi`, intel_pstate (active, HWP-reactive) all confirmed working correctly. Fix: set Power Mode to Balanced (not Power Saver) for daily use; leave cpufreq governor on `powersave` (intel_pstate active mode is reactive, not fixed-low-clock — `schedutil`/`ondemand` unavailable under intel_pstate active). Verified via `stress-ng`: fans ramped audibly at 102–112°C under `performance` governor + non-Power-Saver profile. No throttling/critical events found in dmesg. Full diagnostic trail added to System Setup §.*

*Previous: v99: 12-Factor App pre-commit checklist added as §16 (Fellowship Dev Standards). Mandatory verification before every final git commit on fellowship and Nexus projects.*

*Previous: v98: RF and Microwave Engineering Lab reports added. Lab 1 (ADS intro: DC/AC/parameter sweep) and Lab 2 (impedance matching — quarter-wave transformer 50→150Ω @100MHz; lumped L-section match 15+j10Ω @2.5GHz via Smith Chart Matching Utility, refined to -134dB return loss) both complete. New project ranking entry added (§15).*

*Previous: v97: Nexus Day 4 session complete. T13 (Notes UI) ✅ and T14 (Project system prompt editor) ✅ both implemented and confirmed working. Markdown rendering added (zero-dep `renderMarkdown()` inline parser). Settings text button replaces broken ⚙ glyph. Backend routes `GET/DELETE /projects/{id}/notes/*` and `PATCH /projects/{id}` live. MVP scope table updated. Build log Day 4 entry added.*

*Previous: v96: Nexus §13 updated — Gemini model corrected to `gemini-2.5-flash` (live-confirmed June 13). Both models verified working. MasterPlan_v2 generated (`Plan/Nexus_MasterPlan_v2.md` — 24 tasks, 4 phases). MVP scope table updated to Phase 3/v0.5/v1.0 terminology. Build log Day 3 entry added.*

*Previous: v94 — Added CV & Portfolio sync trigger to Cross-Document Consistency Check section. CV v9 current (Last Updated: June 22, 2026). Portfolio html last-updated date must be verified on upload.*

*Previous: v93 — Fusemachines Week 7 Clustering Assignment marked Complete. Notebook executed end-to-end (S0–S9), repo `fuseAiF_wk7_customer_segmentation` organized (root: executed notebook, PDF, plots/, README, LICENSE, .gitignore with `*.xlsx` ignored; dev artifacts/debug scripts/task plans moved to `misc/` subfolders). Project ranking updated (8.0, Complete). **PORTFOLIO TRIGGER set**: add Week 7 entry to `aaradhyadtmr.github.io` Projects via Decap CMS, matching Week 6 entry style.*

*Previous: v92 — Nexus architecture pivoted from PostgreSQL + ChromaDB to SQLite + FTS5 (v2 redesign). Full backend rewrite (`main.py` — single file, contextmanager DB, FTS5 context injection, key rotation). Frontend redesigned (dark editorial UI, dynamic model columns, Google index routing sidebar). Stack now: React (Vite) · FastAPI · SQLite + FTS5 · httpx · asyncio. Day 2 complete. All Nexus references in profile updated.*

*Previous: v91 — Week 7 Clustering task plan iterated to v3. Gap analysis vs PDF revealed: category spend ratios (keyword-bucketing on Description — 5-category minimum), IQR + Z-score both required for outlier detection, StandardScaler vs RobustScaler explicit decision required (RobustScaler not in S0 imports — needs justification comment per notebook rule). Notebook `.ipynb` read — additional gaps: PDF says `single` linkage, notebook says `average` as 3rd method; resolved by running all 4 dendrograms but fitting only `Hierarchical_Ward` + `Hierarchical_Alt` (matching notebook scaffold column names for S7 compatibility); `Birch` imported in S0 (available for S10); S7 comparison table is 3-row scaffold + optional extras. Final deliverable: `Week7_Clustering_TaskPlan_v3.md`.*

*Previous: v90 — Fusemachines Week 7 Clustering Assignment logged (due June 21, 2026; UCI Online Retail II dataset; K-Means + Hierarchical + DBSCAN pipeline; full task plan `Week7_Clustering_TaskPlan.md` generated; skills added: clustering algorithms, silhouette/Davies-Bouldin/Calinski-Harabasz validation metrics, RFM feature engineering, DBSCAN parameter tuning). Today's exam: O&M Internal Test 1 (June 12, Jestha 29).*

*Previous: v89 — Nexus project added (AI Workflow Hub — personal AI operating system; repo `nexus` under AaradhyaDT; MIT license; React + FastAPI + PostgreSQL + ChromaDB; Day 1 skeleton built; session plan embedded as trigger context).*

*Previous: v88 — PrakopNet BOM updated (RA-02 433 MHz removed → RYLR890 868 MHz adopted; JSN-SR04T replaces HC-SR04; CN3791 replaces TP4056; INA219 added); Nepal LoRa frequency compliance documented (865–867 MHz legal band confirmed); RPi 4B 4GB RAM locked as gateway; feasibility verdict summarised (core demo 80% confidence; 7 additional risk gaps flagged); ChronologicalMerge key doc updated to v3.*

*Previous: v87 — Health diagnosis (chronic allergic conjunctivitis) added; Downloads folder structure documented; C: drive storage analysis noted; HimalGuard_Modifications file removed from key docs (deleted locally); Internal Test 1 context clarified; Ollama model inventory added to System Setup; IDM folder size flagged.*

---

## 📋 Session Loading Instructions

Upload this single file at the start of any Claude session. It contains:
- Full personal & academic identity
- All projects (with CV-accurate descriptions)
- Professional roles & fellowships
- Skills stack & system setup
- Family background & financial context
- Thinking style & Claude preferences
- Ceiling assessment & trajectory planning

### 🔄 Cross-Document Consistency Check (AUTO-TRIGGER)

**When this master profile is loaded alongside any other document, Claude must automatically:**

1. **Scan all uploaded documents** for references that conflict with or predate the master profile's current state
2. **Flag stale references** before proceeding with any task — do not silently use outdated information
3. **Report conflicts** in a brief table at session start: Document | Stale Reference | Current Value in Master

**Known staleness patterns to check for:**

| Check | Current Master Value |
|---|---|
| Project name | **PrakopNet** (formerly HimalGuard — flag any doc still using HimalGuard) |
| Major project direction | Idea D (PrakopNet) confirmed; Idea C (Counter-UAV) archived |
| Major project deadline | **March 2027** (boards/submission); January 2027 = coursework graduation only |
| 8th semester timeline | **Sep 2026 → Mar 2027** |
| Elective I | **EX 725 04 — Aeronautical Telecommunication** (confirmed) |
| Team project roles | PrakopNet roles (see team split table in Major Project §8) — not Counter-UAV roles |
| Masters plan | **Deferred** — only if fully-funded scholarship; not immediate post-graduation |
| Module C PM2.5 | **Included** (reinstated — viable with 6-month timeline) |
| Portfolio hosting | **GitHub Pages.** Multipage migration **complete** (v113). Live-date engine added (v117) — Fuse week, BEI semester, subjects all auto-computed client-side from `new Date()`. Deploy package: `aaradhyadtmr_github_io_v9.zip`. Push checklist: unzip, commit all files, push to `AaradhyaDT/AaradhyaDT.github.io` main. |
| Nexus project | Repo `nexus` under `AaradhyaDT`; MIT; React + FastAPI + **SQLite + FTS5**; Day 1 skeleton June 10, 2026; v2 redesign complete June 12, 2026; T13+T14 done June 13, 2026 |

**Documents most likely to be stale:**
- `PROFILE_AaradhyaDevTamrakar_v4` — roles reference Counter-UAV; needs v5
- `PROFILE_RupeshKadel_v5` — roles reference Counter-UAV; needs v6
- `PROFILE_SankalpaLamsal_v3` — roles reference Counter-UAV; needs v4
- `PROFILE_SoniaThapa_v3` — roles reference Counter-UAV; needs v4
- `PrakopNet_MASTER_v0_20260624.md` — **current operative project truth** (supersedes all ChronologicalMerge docs; generated June 24, 2026)
- `TEAM_PROFILE_SYSTEM_v17_20260610.md` — **current** (TBDs pending June 24 meeting resolution; v11 is stale)
- ~~`MASTER_MajorProject_ChronologicalMerge_v4_UPDATED.md`~~ — superseded by PrakopNet_MASTER_v0
- ~~`HimalGuard_Modifications_v1_20260608.md`~~ — **DELETED locally** (June 10, 2026). Content absorbed into ChronologicalMerge v2 and master profile. No action needed.

**Rule:** If a stale reference is found, flag it and ask whether to update before proceeding. Never silently use the stale value.

### 📅 CV & Portfolio Last-Updated Sync Check (AUTO-TRIGGER)

**When a CV `.docx` or portfolio `.html` file is uploaded, Claude must automatically:**

1. **Check the CV** — find the `Last Updated:` line (bottom of document). Compare against the date of the current session's edits. If it does not match, flag it: `"CV Last Updated reads [date] — update to [today]?"`
2. **Check the portfolio HTML** — find the last-updated or footer date string in the file. Compare against the date of the current session's edits. If stale, flag it: `"Portfolio HTML last-updated reads [date] — update to [today]?"`
3. **Never silently leave a stale date** — both files must reflect the actual date of the most recent edit before being presented as final.

| Asset | Current Last-Updated | Location in file |
|---|---|---|
| CV (`AARADHYA_DEV_TAMRAKAR_CV_vN.docx`) | **June 22, 2026** | Italicised footer line at document end |
| Portfolio HTML (`index.html` or equivalent) | Verify on upload | Footer or meta section — search `last` or `updated` |

### 📅 Temporal Status Verification (AUTO-TRIGGER)

**Every session, before making any claims about what is "active", "current", "in progress", or "complete": check today's date and reason explicitly about whether time-bounded items are actually still ongoing or actually finished.**

**The core failure mode this prevents:** The profile records events by mention — "Wks 1–7 complete", "2026 — Present", "Active — June 2026" — and Claude interprets *mention of completion* as *current status = done*, or interprets *a past start date* as *evidence the thing is still running*. Both errors are wrong. Status must be derived from the date, not from the label.

**Trigger procedure (run at session start, silently — only surface findings that affect the task):**

1. **Get today's date.** It is always available from the system context. Use it. Do not estimate or assume.

2. **Scan these temporal patterns in the profile and reason about each:**

| Pattern | Rule |
|---|---|
| `[Role/Item] — [Year] — Present` | Verify: is this role confirmed current? Check if there is a known end date or semester boundary that has since passed. Do not assume "— Present" is still true just because it was written that way. |
| `[Item] — Wks N complete` or `[N] weeks done` | This means N weeks are done. It does NOT mean the fellowship/program is finished. Check if there is a known total duration or end date and compare to today. |
| `[Item] — Active — [Month Year]` | Check if that month has passed. If it has and no completion entry exists, flag as "status unknown — may be stale". |
| `Semester [N] — [Month Range]` | Check whether today's date falls inside or outside the semester window. Do not infer semester from academic year label alone. |
| `Expected [graduation/completion/deadline]: [Date]` | Compare to today. If the date is past, flag the item as likely complete or overdue. If it is future, it is still pending. |
| `Deadline: [Date]` | If the date is past and no completion note exists, flag as "deadline passed — outcome unknown". |
| `[Item] *(Active — [Date])*` or `*(In Progress)*` without a date | Treat as unverified. Do not infer complete or ongoing without explicit date evidence. |

3. **Apply the corrected status when generating any response.** If the profile says "Fuse AI Fellowship — Wks 1–7 complete" and the fellowship has a known 7-week structure with a start date, calculate whether 7 weeks from start date has passed and report accordingly. If the profile says "2026 — Present" for a role but the semester in which that role was held ended before today, flag it.

4. **Do not silently correct.** If temporal reasoning produces a different status than what is written in the profile, surface the discrepancy before acting on it: `"Profile reads [X] but today is [date] — treating as [Y]. Confirm?"`

5. **Never treat mention as completion.** Recording that something happened ("Wk 7 done", "Lab 2 complete") is a milestone log, not a terminal status. A program with 7 weeks done is complete only if 7 weeks = the full program length AND the end date has passed.

**Common cases to always check:**
- **Fusemachines AI Fellowship:** 24-week structure (6 months). Start: May 4, 2026. End: Oct 18, 2026. Current week = `floor((today − May 4 2026) / 7) + 1`, capped at 24. Do not infer "complete" before Oct 18, 2026.
- **NSSR DataCamp Fellowship:** Phase 1 done; Phase 2 active. Ongoing until told otherwise.
- **IEEE KEC KTM roles:** Term-bound by academic year (Sep–Aug). Do not assume expired without explicit end date.
- **BEI semester (critical):** IV/I = 7th semester. IV/II = 8th semester. **Semester boundary is not the exam date** — it is the official KEC semester transition (~Sep). Completing IV/I exams does not make Aaradhya IV/II until 8th semester formally begins (Sep 2026). If today < Sep 2026, Aaradhya is IV/I.
- **PrakopNet proposal deadline:** July 2, 2026. If today is past this, flag as "deadline passed — confirm outcome."
- **8th semester start:** Sep 2026. If today < Sep 2026, it has not started.

### 💡 Claude Pro ROI (AUTO-TRIGGER)

**When Aaradhya mentions "Claude Pro ROI" in any session, Claude must automatically do all three of the following:**

1. **Surface what the profile says** — read and summarize the current state from `### Planned Subscriptions` and `### Claude Pro ROI Assessment` in the Banking & Subscriptions section. Report: subscription status, payment path, activation trigger, and any blockers logged.

2. **Ask for current context + suggest simultaneously** — in the same response, ask which of these is most active right now: (a) still saving/planning, (b) dollar card access confirmed, (c) GitHub Edu Pack result known, (d) already subscribed. Without waiting for the answer, simultaneously suggest the most relevant next action given the profile's current trajectory (Fusemachines fellowship, Nexus dev, PrakopNet thesis, student window expiry).

3. **Apply Claude/AI ecosystem expert knowledge** — draw on best-practice knowledge of the Claude product ecosystem (Pro vs API vs Claude Code use cases, Projects feature, token economics, student window timing) to give forward-looking strategic advice tailored to Aaradhya's actual workload and 1–2 year student account window. Think ahead: what should be learned in what order, what free alternatives to exhaust first, how to sequence Pro → Claude Code → API for maximum career ROI before graduation (Jan 2027) and before student account expires.

**This trigger fires on any mention of "Claude Pro ROI" — even mid-task. Complete the three steps before returning to the original task.**

### 🤝 Fellowship Priority Trigger (AUTO-TRIGGER)

**Activation signals — any one is sufficient:**
- Repo or file name matches `fuseAiF_*` pattern (e.g. `fuseAiF_wk8_nlp`, `fuseAiF_wk9_*`)
- User says "fellowship", "Fusemachines", "fuse week", or mentions a week number in a Fusemachines context
- A `PATCH_fuse*.md` file is uploaded alongside the master profile
- Secondary triggers (also activate fellowship mode): CV update, portfolio HTML update, LinkedIn update

**When triggered, Claude must — in order:**

1. **Load fellowship context first.** Before any task output, silently check:
   - Current Fuse week: `floor((today − May 4 2026) / 7) + 1`, capped at 24. Today is June 26, 2026 → **Wk 8/24**.
   - Which week's repo this session is about (from filename or user message).
   - Whether a `PATCH_*.md` was uploaded — if so, treat it as the primary source of session truth for that week's work.

2. **If a PATCH file is present**, run patch-merge mode:
   - Read patch meta (source repo, period, generated-by, sections affected).
   - Apply new facts to the relevant §Projects entry and §Fellowship history.
   - Flag any deprecations/corrections against current master values.
   - Produce updated master version with changelog entry.

3. **If no PATCH file**, run standard fellowship session mode:
   - Ask whether this session will produce a patch (at end of session, offer to generate patch summary).
   - Apply 12-Factor pre-commit checklist gate (§16) before any `git commit` advice.
   - Track task completion against the week's assignment scope.

4. **Speed-replay awareness.** Any work done this session that involves a new repo, notebook, or deliverable should be summarised at session end in patch-ready format (what was done, what was built, what was learned, mistakes, open items) so it can be fed to a large-context AI to generate the formal `PATCH_*.md`.

5. **Naming convention for patch files:**
   - `PATCH_fuseWkN_[topic]_YYYYMMDD.md` — e.g. `PATCH_fuseWk8_nlp_20260626.md`
   - `PATCH_portfolio_YYYYMMDD.md` — for portfolio/CV/LinkedIn updates
   - Always include: source repo, period, generated-by, sections affected, what was done, what was built, what was learned, mistakes/corrections, open items, evidence pointers (commit hashes, notebook cells, key metrics).

---

## 📦 §17 — Patch System: Documentary Update Protocol

### Purpose

Repos for fellowship weeks, PrakopNet, and Nexus accumulate many files quickly. A large-context AI (Gemini 2.5 Pro, GitHub Copilot) can read an entire repo in one pass and extract a structured documentary — a **patch** — capturing what happened. Patches serve two purposes:
1. **Master profile updates** — Claude merges patch facts into the relevant §§ without re-reading the full repo.
2. **Speed-replay log** — 2–3 minute read to fully reconstruct a week's work months later.

### Patch Template (`PATCH_[source]_[YYYYMMDD].md`)

```md
# PATCH — [repo name or source] — [YYYY-MM-DDTHH:MM+05:45]

## Meta
- Source repo: [e.g. fuseAiF_wk8_nlp]
- Period: [start date] to [end date]
- Generated by: [Gemini 2.5 Pro / GitHub Copilot / manual]
- Master profile sections affected: [e.g. §Projects > Wk 8, §Skills > NLP]

## What Was Done
- [Concrete task — tool used, dataset, method, outcome]
- [Concrete task 2]

## What Was Built
- [filename]: [what it does, key metric if applicable]
- [filename]: [what it does]

## What Was Decided / Learned
- Chose [X] over [Y] because [reason from commit message or comment]
- Key insight: [1-line takeaway]

## Mistakes / Corrections
- First attempt used [wrong approach] → fixed by [fix]

## Open Items Carried Forward
- [ ] [Task not completed — deferred to next week or session]

## Evidence Pointers
- Commit: [hash] — "[message]"
- Notebook cell [N]: [what it shows]
- Key metric: [e.g. F1: 0.87, Silhouette: 0.54]
```

### Gemini / Copilot Extraction Prompt

Paste this verbatim when asking a large-context AI to generate a patch from a repo:

> *"You are a knowledge extractor. Read the entire repository I have attached. Fill the patch template below with: (1) concrete facts about what was done — exact filenames, metric values, dataset names, tool choices, commit messages, decisions visible in comments or READMEs; (2) what was built and its key outputs; (3) key decisions and the reasoning behind them; (4) mistakes made and how they were corrected; (5) open items not completed. Be specific — the reader is the person who built this, reviewing it 6 months later. Do not generalize or summarize abstractly. Cite the file and cell/line for each fact where possible. Output only the filled patch template in Markdown."*

Then append the patch template above.

### Claude Merge-Session Prompt

When bringing patches to Claude alongside the master profile:

> *"I'm uploading AARADHYA_MASTER_vN.md and the following patch files: [list]. Please merge each patch into the master profile — update the relevant §Projects entries, §Skills if new tools appear, and §Fellowship history. Add a v(N+1) changelog entry summarising what changed. Flag any patch facts that conflict with current master values before merging."*

### Workflow Summary

```
Repo (commits, notebooks, READMEs, code)
    ↓
Large-context AI (Gemini 2.5 Pro / Copilot)
  + Extraction prompt above
    ↓
PATCH_fuseWkN_[topic]_YYYYMMDD.md

[Later — any session]
MASTER_vN.md + PATCH_*.md(s)
    ↓ Claude merge session
MASTER_v(N+1).md  ←  updated, versioned, timestamped
                  ←  also usable standalone as speed-replay log
```

---

## 🏦 Banking & Subscriptions

### Siddhartha Bank (SBL)
| Item | Detail |
|---|---|
| **Account** | GenZ Account (active) |
| **Dollar card** | SBL E-com Card (plan: apply at branch) |
| **E-com Card fee** | NPR 500 (1st issuance), NPR 250 reload (2nd+ load) |
| **E-com Card limit** | USD 500/year (resets from first transaction date) — online foreign payments only, no ATM/POS |
| **Docs needed** | Citizenship + PAN + GenZ account details + application form at branch |

### Planned Subscriptions
| Service | Cost | Status | Notes |
|---|---|---|---|
| **Claude Pro** | ~$20/month (~$240/year) | Saving up — not yet subscribed | Primary: trusted contact's dollar card; SBL E-com Card as fallback (~$240 of $500/year limit); GitHub Edu Pack applied (may unlock Anthropic API credits) |
| **GitHub Education Pack** | Free | Applied — pending approval | Unlocks GitHub Copilot, GitHub Pro, and potentially Anthropic API credits |

### Claude Pro ROI Assessment
| Factor | Detail |
|---|---|
| **Break-even** | Save ~1 hour/month at any billable rate to justify cost |
| **Primary use cases** | Nexus dev (code/debug), PrakopNet thesis (LaTeX/docs), Fusemachines assignments, exam prep hubs, CV/portfolio iteration |
| **Current bottleneck** | Free tier worked to maximum capacity across all active workstreams |
| **Student window** | 1–2 years of student account validity remaining — binding constraint on free/discounted access |
| **ROI verdict** | High — free tier exhausted; Pro's 5× capacity + Claude Code + API fluency = career differentiator before Jan 2027 graduation |
| **Activation trigger** | Subscribe when trusted contact's dollar card access confirmed; SBL E-com Card or GitHub Edu Pack as fallback |
| **Learning sequence** | Pro chat + Projects (Week 1) → Claude Code on Nexus/PrakopNet (Week 2–3) → API automation (Month 1) |

### Effort Level & Thinking Mode — Optimal Usage Guide

**Two independent controls in Pro UI:** Effort (Low / Medium / High / Max) + Thinking toggle (On / Off). Combine them deliberately — running Max + Thinking on everything burns 3–10× tokens and will cut Pro's ~40–80 msg/5hr window to ~10–15 exchanges.

**Default rule: High effort, Thinking OFF. Flip Thinking ON only for stuck/irreversible/multi-step numerical work.**

| Task | Effort | Thinking | Reason |
|---|---|---|---|
| Quick lookups, Q&A, single-file edits, CV/profile updates | Low | OFF | Mechanical — save quota |
| Master profile updates, exam prep hub generation, LaTeX/thesis writing | High | OFF | Structured output — speed > deliberation |
| Nexus debugging (known error, specific bug) | High | OFF | Pattern recognition — overthinking hurts |
| Fusemachines assignments (data pipelines, clustering, ML tasks) | High | ON | Multi-constraint problems benefit from deliberation |
| Nexus architecture decisions (e.g. FTS5 vs vector store, API design) | Max | ON | Trade-off analysis, many variables, correctness matters |
| PrakopNet system design (LSTM architecture, HazardScore fusion) | Max | ON | High correctness-critical, multi-variable |
| RF/Smith chart / numerical problem solving | Max | ON | Sequential numerical reasoning — thinking catches mid-chain errors |
| Creative/prose writing | High | OFF | Thinking degrades intuitive writing quality |

**Token cost reality:** Thinking burns 3–10× tokens per call vs standard. On the wrong task it's slower and gives the same answer. On the right task (architecture, debugging a hard logic error, multi-step math) it's the difference between a correct and incorrect result.

**One habit that stretches Pro 3–5× further:** Default High/OFF → escalate to Max/ON only when stuck or making an irreversible decision.

---

## 🔑 Accounts & Identities

| Account | Email |
|---|---|
| **Primary (Claude — active)** | aaradhyadevtmr@gmail.com |
| Claude (secondary) | devtamrakaraaradhya83@gmail.com |
| Claude (alt) | xavier.valois007@gmail.com |
| **Claude (Major Project)** | majorprj79001@gmail.com |
| ChatGPT / GPT-5.3 | aaradhyadevtmr@gmail.com |
| IEEE | aaradhya.devtamkarar@ieee.org |
| Family | tamrakarfamily0@gmail.com |
| Gaming / Misc | adtgames2061@gmail.com |

### Major Project Group Accounts
| Member | Gmail | Notes |
|---|---|---|
| Aaradhya (project Claude) | majorprj79001@gmail.com | Claude account for Major Project workstream |
| Rupesh Kadel | majorprj79034@gmail.com | Has own personal account too |
| Sankalpa Lamsal | majorprj79039@gmail.com | Has own personal account too |
| Sonia Thapa | majorprj79043@gmail.com | Has own personal account too |

> Maintains Claude accounts for parallel workstreams. Uses `.md` files for cross-session continuity.

---

## 🧑 Personal Identity

| Field | Details |
|---|---|
| **Full Name** | Aaradhya Dev Tamrakar[cite: 9] |
| **Date of Birth** | January 6, 2005 (Friday, 11:45 PM)[cite: 9] |
| **Birthplace** | Chitwan, Nepal[cite: 9] |
| **Current Location** | Kathmandu, Bagmati Province, Nepal (KEC Boys' Hostel, on-campus)[cite: 9] |
| **Ethnicity** | Newar (Tamrakar)[cite: 9] |
| **Family Roots** | Patan (grandfather's origin, near Krishna Mandir), Jhapa (2 pieces of land in Damak — illiquid)[cite: 9] |
| **Phone** | +977 9844602050[cite: 9] |
| **LinkedIn** | linkedin.com/in/aaradhya-dev-tamrakar[cite: 9] |
| **GitHub** | github.com/AaradhyaDT[cite: 9] |
| **Portfolio** | aaradhyadtmr.github.io (GitHub Pages, multipage static site — v7 build complete, not yet pushed; single-file `index.html` still live until v7 push)[cite: 9] |

### Vedic Astrology

| | |
|---|---|
| **Rashi** | Vrischik (Scorpio) — Scorpio Moon[cite: 9] |
| **Lagna** | Kanya (Virgo)[cite: 9] |
| **Nakshatra** | Rohini[cite: 9] |
| **Mahadasha** | Rahu Mahadasha (Jan 2022 – Jan 2040)[cite: 9] |

### Planetary Positions

| Planet | Rashi | Degrees |
|--------|-------|---------|
| Lagna | Kanya (Virgo) | 15° 43' 16"[cite: 9] |
| Surya (Sun) | Dhanu (Sagittarius) | 22° 36' 48"[cite: 9] |
| Chandra (Moon) | Vrischik (Scorpio) | 0° 16' 6"[cite: 9] |
| Mangal (Mars) | Vrischik (Scorpio) | 14° 24' 17"[cite: 9] |
| Budha (Mercury) | Dhanu (Sagittarius) | 1° 30' 11"[cite: 9] |
| Vrihaspati (Jupiter) | Kanya (Virgo) | 23° 52' 36"[cite: 9] |
| Shukra (Venus) | Dhanu (Sagittarius) | 2° 23' 5"[cite: 9] |
| Shani (Saturn) | Karkat (Cancer) | 0° 33' 26"[cite: 9] |
| Rahu | Mesh (Aries) | 4° 52' 31"[cite: 9] |
| Ketu | Tula (Libra) | 4° 52' 31"[cite: 9] |

### House Placements

| House | Sign | Planets |
|-------|------|---------|
| 1st (Lagna) | Kanya (Virgo) | Jupiter ♃[cite: 9] |
| 2nd | Tula (Libra) | Ketu[cite: 9] |
| 3rd | Vrischik (Scorpio) | Moon + Mars[cite: 9] |
| 7th | Meena (Pisces) | Rahu[cite: 9] |
| 10th | Mithun (Gemini) | Saturn[cite: 9] |
| 12th | Simha (Leo) | Sun + Mercury + Venus[cite: 9] |

### Chart Highlights

- **Kanya Lagna + Jupiter in 1st house** — methodical, detail-oriented, service-driven[cite: 9]
- **Moon + Mars conjunct in Scorpio (3rd house)** — intensity, willpower; internalizes until eruption[cite: 9]
- **Sun, Mercury, Venus in 12th house** — processes alone before externalizing; inner life dominates[cite: 9]
- **Rahu in 7th house** — karmic/unusual relationships; 18-year amplification period[cite: 9]
- **Saturn in 10th house** — career earned methodically, not gifted; slow but solid builder[cite: 9]

---

## 👨‍👩‍👦 Family Background

| Member | Age | Role / Status |
|---|---|---|
| **Father** | 53 | Senior Agency Manager, NLIC — client acquisition increasingly difficult[cite: 9] |
| **Mother** | 48 | Part-time health screening associate, IOM[cite: 9] |
| **Brother** | 15 | Just completed SEE; moving to Kathmandu for +2 Science (Computer)[cite: 9] |

- 2 pieces of land in **Damak, Jhapa** — family asset, illiquid[cite: 9]
- **Financial position:** Constrained but stable[cite: 9]. No significant safety net[cite: 9]. Brother arriving adds household pressure[cite: 9].
- **Time horizon:** ~2–3 year window before family expects financial contribution[cite: 9]. Not crisis — but a real clock[cite: 9].

### Generational Context

**Father's side:**
- Wealthy 4+ generations back
- Grandfather was the only son — yet received no inheritance
- Multiple stepmothers entered one after another (fates unconfirmed — left or deceased)
- Stepmother abuse forced grandfather to relocate to Chitwan; inheritance severed entirely despite being the sole male heir
- Root cause: outsider entry → abuse/exclusion → inheritance chain broken

**Mother's side:**
- Wealthy 4+ generations back; poverty hit ~2 generations ago
- Great-grandmother was the 2nd wife — 1st wife had no children; 3rd wife drove the others out, cutting off family support and inheritance
- Root cause: same mechanism — outsider entry → exclusion → inheritance chain broken

**Pattern recognized across both sides:**
- Identical failure mode, independently on both family lines: an external entrant chose exclusion/abuse over family continuity, severing generational wealth at a single inflection point
- Not bad luck — deliberate acts of exclusion repeated across both lineages
- Aaradhya consciously identifies as the generation that breaks this cycle on both lines

- **Loyalty hierarchy:** Immediate family of four → close friends → reciprocal cousins → behavior-based acquaintances[cite: 9]. Extended family who were extractive: no obligation[cite: 9].
- **Marriage approach:** Court marriage first, small celebration, closest only[cite: 9].

### Health

| Condition | Detail |
|---|---|
| **Chronic Allergic Conjunctivitis** | Left eye primarily; diagnosed June 10, 2026. Red eye recurring ~monthly since Falgun (Feb 2026), alternating eyes. Treatment: antihistamine eye drops (use on schedule, not just on flares). Screen-heavy sessions aggravate it. |
| **Eye care note** | Hostel environment (dust/shared spaces) is a common trigger. Avoid rubbing. Pillow hygiene matters. |

---

## 🎓 Academic Background

| Field | Details |
|---|---|
| **Institution** | Kathmandu Engineering College (KEC), IOE, Tribhuvan University[cite: 9] |
| **Degree** | Bachelor of Electronics, Communication and Information Engineering (BEI)[cite: 9] |
| **Current Level** | Year IV / Part I — 7th Semester[cite: 9] |
| **Expected Graduation** | January 2027[cite: 9] |

### Current Subjects (IV/I — 7th Semester)
Wireless Communication · Artificial Intelligence · Organization & Management · Digital Signal Analysis & Processing · RF & Microwave Engineering · **Elective I: EX 725 04 — Aeronautical Telecommunication** ✅ (confirmed) · Project Part A

> **Elective I — CNS alignment confirmed.** Aeronautical Telecommunication covers ATC communications, ILS/VOR/DME/NDB navigation aids, surveillance systems (SSR, ADS-B), ICAO standards, and CNS/ATM frameworks — directly maps to CAAN Nepal and AAI India JE career target. Exam: June 22, 2026.

### IV/II Subjects (8th Semester — incoming, Sep 2026)
Telecommunications · Professional Practice · Energy, Environment and Society · Information Systems · Elective II (EX 765) · Elective III (EX 785) · Project Part B (Major Project — PrakopNet, deadline March 2027)

> **IV/II Elective strategy (confirm at registration):** Two elective slots. Given CNS/aeronautical path and PrakopNet: Elective II → **Radar Technology (EX 725 01)** or **Satellite Communication (EX 725 02)** if available for IV/II slot. Elective III → **Data Mining (CT 785 02)** (supports PrakopNet ML analytics) or **Remote Sensing (CT 785 01)** (supports GIS/geospatial angle for PrakopNet commercialization). Confirm which options KEC offers for IV/II at registration.

### IV/I Exam Schedule (2083 — Test 1)
> **Internal Test 1 context:** Limited syllabus coverage (not full boards). Questions are provided in advance for each subject. Preparation strategy = know the given questions cold, not cover the full syllabus.

| Date (BS) | Date (AD) | Subject |
|---|---|---|
| Jestha 22 | Jun 5 | Wireless Communication ✅ |
| Jestha 25 | Jun 8 | Artificial Intelligence ✅ |
| Jestha 29 | Jun 12 | Organization & Management — outcome not logged |
| Asar 1 | Jun 15 | Digital Signal Analysis & Processing — outcome not logged |
| Asar 5 | Jun 19 | RF & Microwave Engineering — outcome not logged |
| Asar 8 | Jun 22 | Elective I — EX 725 04 Aeronautical Telecommunication ✅ |
| Asar 12 | Jun 26 | Project Part A (no written exam) ← TODAY — outcome not yet logged |

### Study Resource Assets (assembled June 2026)
- **IV/I Syllabus** — `BEIE_IV_I_Syllabus.md` (all 7 subjects, full topic breakdown)
- **IV/II Syllabus** — `BEIE_IV_II_Syllabus.md` (all 7 subjects, full topic breakdown)
- **Full BEI Curriculum** — `BEI_Curriculum_ElectronicsCommunicationInformation.md` (all 8 sems, credit hours, marks)
- **All 8-semester subject PDFs** — individual syllabus PDFs for every semester; self-collected (not provided at orientation)
- **Past questions** — downloaded past exam papers for IV/I subjects
- **Study hub template** — `es_ct655_integrated.html` — single-file HTML exam prep hub (CT 655, III/II). Method confirmed effective. Template for IV/I subject hubs.

### Study Hub Method (from CT 655 / III/II finals)
Single-file HTML per subject: Q-sections mapped to exam slots, frequency map, predictions, past papers, Q&A, quiz, reading roadmap. Method fit for IV/I:

| Subject | Fit | Notes |
|---|---|---|
| Artificial Intelligence | Excellent | Fixed topic slots, same pattern as CT 655 |
| Org & Management | Excellent | Pure written, predictable |
| Wireless Communication | Good | Needs formula banks added |
| DSAP | Good | Needs solved-numericals section per topic |
| RF & Microwave | Good | Needs worked examples for circuit analysis |

### BEI Curriculum Coverage (Full — for project framing)

| Domain | Subjects |
|---|---|
| Core Electronics | Basic Electronics, Electronic Circuits, Analog & Digital Communication, Microprocessors & Microcontrollers, VLSI & IC Design, Power Electronics[cite: 9] |
| Communication & RF | Communication Systems, Propagation & Antenna, Fiber Optics, Satellite & Mobile Communication, Transmission Lines & Waveguides[cite: 9] |
| Information / Software | Data Structures & Algorithms, Computer Networks & Security, DBMS, OS, OOP, Web Technology[cite: 9] |
| Signal Processing & Math | Signals & Systems, Digital Signal Processing, Engineering Mathematics I–IV, Probability & Stochastic Processes[cite: 9] |
| Control & Instrumentation | Control Systems, Instrumentation & Measurement, Sensors & Transducers[cite: 9] |
| Applied | Minor Project (GCSBR) · Major Project[cite: 9] |

---

## 💼 Professional & Organizational Roles

| Role | Organization | Period |
|---|---|---|
| **Fuse AI Fellow** | Fusemachines | May 4 2026 – Oct 18 2026 (24 wks / 6 months); Wk 8/24 as of June 25 2026 |
| **Vice Chair** | IEEE KEC Student Branch | 2026/2027[cite: 9] |
| **DataCamp Fellow — Cohort 2** | NSSR | 2026–Present[cite: 9] |
| **Event Manager** | Electronics Project Club (EPC), KEC | 2026–Present[cite: 9] |
| **Vice Secretary** | IEEE KEC Student Branch | 2025–2026[cite: 9] |
| **Resource Manager** | Electronics Project Club (EPC), KEC | 2024–2026[cite: 9] |
| **Makerspace Ambassador** | KEC Maker's Space | June 2026–Present (web dev track; grants free 3D printing, laser cutting, materials, 1Gbps WiFi). Active deliverable: `KEC-innovation/makerspace-main` site fixes shipping since June 17, 2026 — see § KEC Makerspace Website. |
| **Charter Membership Chairperson** | LEO Club of Damak Gold | Jan 2020 – 2025 (disbanded)[cite: 9] |
| **2nd Vice President** | LEO Club of Damak Gold | May 2020 – May 2021 (1 yr 1 mo)[cite: 9] |

### 🏢 Screened Opportunities

| Company | Role | Stage Reached | Outcome | Notes |
|---|---|---|---|---|
| **eSewa (F1Soft Group)** | QA Intern | Written exam ✅ | Not selected — full-time commitment conflict | CV forwarded to eSewa sister organizations (F1Soft Group) per exam results; passive pipeline open. Results: June 2026. |

---

## 🌐 Actual Situation & Path (as of June 2026)

*This section is the ground truth. Not a task log — the real picture.*[cite: 9]

### Where things stand

Aaradhya is 21, finishing BEI at KEC (graduation Jan 2027), with ~2–3 years before the family financial clock becomes a crisis[cite: 9]. He has built a stronger portfolio than most BEI students at his level — real shipped work, not just coursework — but his core gap is **finishing things**[cite: 9]. The gap between what he starts and what ships is the main ceiling limiter[cite: 9]. Completion is the only metric that matters right now[cite: 9].

He is mid-Rahu Mahadasha (through Jan 2040) — the period of maximum amplification[cite: 9]. High upside and high volatility[cite: 9]. Every decision this decade compounds[cite: 9].

### The actual path

**Clarified future goals (June 8, 2026 — in order of execution):**

1. **Fuse AI Fellowship completion** — primary focus through mid-2026. Highest CV leverage. Every week's output must be real, understood code.
2. **Graduate as BEI engineer** — Jan 2027 (coursework complete); boards/project submission March 2027. PrakopNet demo in hand.
3. **CNS/aeronautical engineering role** — post-graduation primary income path. CAAN Nepal or AAI India (Junior Executive – Electronics exam). Directly leverages RF & Microwave, signal processing, embedded background. NEC 97/100 mock score = exam-ready.
4. **PrakopNet commercialization** — post-graduation side track alongside job. First pilot: municipality, NGO, or hydropower operator. Makerspace fabrication resources make the hardware demo professional-grade.
5. **Masters** — deferred. Only viable if fully-funded scholarship (MEXT, DAAD, Erasmus Mundus) appears. Unfunded masters during the financial clock window is high-risk and competes directly with PrakopNet momentum. Target Year 3–5 post-graduation, with 2–3 years of domain context making the research output stronger.

**Phase map:**

| Phase | Period | Primary | Secondary | Background |
|---|---|---|---|---|
| Exam period | May → Jun 26 | **IV/I exams complete** — Project Part A today (Jun 26, outcome not yet logged) | Fellowship (weekly deadlines hold it) | Makerspace web dev, Excelerate application |
| Fellowship final stretch | Jul → Aug 2026 | Fellowship completion | Excelerate internship (if matched) | PrakopNet architecture, DataCamp |
| 8th semester | Sep 2026 → Mar 2027 | PrakopNet demo | NEC license prep | DataCamp certs, IEEE events |
| Post-graduation | Mar → Aug 2027 | Job applications (CNS + AI/ML) | PrakopNet pilot/grant push | Upwork profile (portfolio now complete) |
| Year 1–3 | 2027–2030 | CNS/engineering job | PrakopNet commercialization | Masters prep (if funded path appears) |

**Time slot rule (completion gap countermeasure):**
One primary. One secondary. Background only for things that run themselves. Nothing enters the primary slot until the current primary ships or has an immovable external deadline. This is the structural fix for the known commitment-stacking pattern. Fellowship deadlines are the proof it works — same forcing function must be replicated for every new commitment.

**Earning timeline:**

| Milestone | Target | Earning |
|---|---|---|
| Excelerate application | This week (apply now, start Jul) | Structured project, possible pay, CV line |
| Fellowship completes | Mid-2026 | GitHub portfolio live and visible |
| PrakopNet demo | Mar 2027 | Grant applications competitive; pilot conversations viable |
| Post-graduation job | Jan–Jun 2027 | Rs. 40–70k/month Nepal / ₹6–12 LPA India |
| PrakopNet pilot | Year 1–2 | NGO grant or municipal contract upside |
| Upwork side income | Year 1 (job stable) | Rs. 15–25k/month supplementary |

**Excelerate + OpportunitiesRadar:**
- Excelerate: virtual project-based internships, 4–8 week commitments. Target: AI/ML pipeline or IoT projects. Apply this week; start July post-exams. "Intern at [Company]" reads better than "Freelancer" for CNS/engineering job applications.
- OpportunitiesRadar: discovery aggregator only. Use weekly to find Nepal-relevant AI/ML, IoT, disaster tech internships and PrakopNet-relevant grant calls.

**Phase 1 — Now to March 2027 (before graduation/boards)**[cite: 9]

The goal is to graduate with a CV that can compete for ML/AI engineering roles at ₹6–12 LPA entry (India is one option under active consideration — not confirmed), and build enough credential mass that any post-graduation move is justified rather than a leap into the dark[cite: 9].

What's currently running:
- **Fusemachines AI Fellowship** (the primary focus): 24-week program (May 4 – Oct 18, 2026); currently Wk 8/24, ongoing[cite: 9]. This is the most valuable thing on the CV right now[cite: 9]. Every week's output needs to be real, understood code — not copy-pasted[cite: 9]. Fellowship ends Oct 18, 2026[cite: 9].
- **Portfolio website**: `aaradhyadtmr.github.io` — multipage architecture (`index.html`, `projects.html`, `experience.html`, `achievements.html`, `about.html`, `contact.html`), static HTML/CSS/JS on GitHub Pages. The Netlify + Decap CMS migration explored June 10, 2026 was cancelled at v111 — site remains static, no CMS layer, no `/admin/`, no JSON content files.
- **IEEE KEC Vice Chair**: Running real events[cite: 9]. SPAx "Engineer Your Profile" happened May 23[cite: 9]. The risk is it becomes a title without substance — must run something that leaves a mark[cite: 9].
- **Major Project — PrakopNet** (Idea D, confirmed June 8, 2026): Solar-powered LoRa mesh multi-hazard EWS. Demo target: **March 2027 boards**. Makerspace Ambassador access (3D printing, laser cutting, 1Gbps WiFi) directly supports hardware fabrication. See Major Project section for full spec.[cite: 9]
- **DataCamp certs** (NSSR fellowship): Fully completed Phase 1 Applied AI portfolio[cite: 3, 5, 8]. Transitioning to SQL Associate + Python Data Associate pathways[cite: 8]. Data Engineer + Data Scientist + AI post-fellowship[cite: 9]. Background resource — zero conflict with Fusemachines[cite: 9].
- **Algoverse AI Research application**: Deadline May 24, 2026 — **passed, outcome not logged[cite: 9].** Research problem: "Efficient Multimodal Reasoning on Edge Devices: Quantization Strategies for Real-Time Gesture Recognition Using Optimized LLMs[cite: 9]." Grounded in live DeepSeek R1 7B on Intel Arc + GCSBR[cite: 9]. Cohort (June–Aug 2026) is currently running — if accepted, this is a concurrent full-time 8–12 week commitment that should be confirmed and reconciled against current Fellowship/exam load[cite: 9]. Targets NeurIPS edge ML workshops / ACL efficiency track[cite: 9].

What's been cancelled or deprioritized:
- **Robotica 6-Month Robotics Technician Program**: Cancelled[cite: 9]. Morning batch conflict, budget, and Algoverse opportunity made it the right cut[cite: 9].
- **eSewa Android Intern**: Applied May 13[cite: 9]. Outcome unknown[cite: 9]. If not selected: no disruption — it was an opportunistic application, not the plan[cite: 9].
- **eSewa QA Intern**: Written exam passed. Not selected — full-time commitment conflict. CV forwarded to F1Soft sister organizations. Results: June 2026. Passive pipeline open.

**Phase 2 — Post-graduation (March 2027 onward)**[cite: 9]

**Primary career target: CNS/aeronautical engineering.** RF & Microwave, signal processing, embedded systems background maps directly to CNS ground infrastructure (VHF/UHF comms, ILS, DVOR, SSR, ADS-B, MLAT). NEC mock score 97/100 = exam-ready.

- **Nepal:** CAAN (Civil Aviation Authority of Nepal) CNS/electronics roles — stable, government-adjacent, limited openings per year.
- **India:** AAI Junior Executive (Electronics) — written exam path, tens of openings, BEI + NEC qualifies directly. Bangalore / Pune / Hyderabad under consideration.
- **AI/ML engineering roles:** Fusemachines fellowship credential is the pitch. ₹6–12 LPA entry India.

Strategic alignment: CNS job + PrakopNet are synergistic. Day job builds domain relationships with the same infrastructure operators who are PrakopNet's target customers (DHM, CAAN-adjacent, telecom serving remote areas).

**Masters:** Deferred unless fully-funded scholarship. Without funding: wait until Year 3–5. A thesis on edge AI for disaster EWS at that point upgrades PrakopNet's research novelty score (7.5 → 9+) and builds international fundraising network. Better research output with 2–3 years of domain experience behind it.

NI cert sequence (if AI/ML engineering path): CLAD post-fellowship (mid-2026, 6 mo LabVIEW practice) → CTD simultaneously → CLD (Year 2–3) → branch to CLED or CTA depending on first job domain[cite: 9].

### The honest constraints

- **Completion gap**: Starts well, loses momentum[cite: 9]. SysOptimizer v5, Alpha app, portfolio site fixes — all partially done[cite: 9]. The pattern is known[cite: 9]. Fellowship deadlines are the only structure that's been reliably closing things[cite: 9].
- **Financial clock**: Not crisis yet[cite: 9]. But the window is real[cite: 9]. Earning before graduation (Rs. 15–20k/month) changes psychological position significantly[cite: 9].
- **No shortcuts on understanding**: AI/local LLM environment is set up[cite: 9]. The risk is using it as a crutch rather than a tool[cite: 9]. The fellowship work has been done with genuine understanding — that needs to stay true[cite: 9].

### What would constitute success by March 2027

1. Next-gen applied GenAI competencies locked via structured training pipelines[cite: 3, 5].
2. Fusemachines fellowship completed with public GitHub deliverables for every week — visibly real work[cite: 9]
3. Major Project functional demo — runs, not just documented[cite: 9]
4. Alpha on Play Store **or** one DataCamp career cert[cite: 9]
5. Post-graduation plan concrete: offer in hand, or strong pipeline of applications[cite: 9]

---

## 🛠️ Projects

### 1. Gesture-Controlled Self-Balancing Robot (GCSBR) — Minor Project *(Completed)*
**Stack:** Computer Vision · Arduino · MPU6050 · Stepper Motors · Android · MATLAB[cite: 9]
**Rating: 9.4/10 — Examiner called it "major project level"**[cite: 9]

- Sensor fusion + PID stabilization + mobile gesture control[cite: 9]
- Firmware V6.9.1: watchdog timer, atomic writes, differential ramp, integrator bleed[cite: 9]
- MATLAB simulation → real-world hardware deployment[cite: 9]
- Android gesture-control interface (MediaPipe, CameraX, HC-05 BT)[cite: 9]
- Dual-hand gesture control; DRV8825 drivers on CNC Shield[cite: 9]
- GitHub: `AaradhyaDT/Gesture-Controlled-Self-Balancing-Robot`[cite: 9]

### 2. Text-to-SQL Agentic Pipeline (Fusemachines Week 3) *(Completed)*
**Stack:** Python · FastAPI · Streamlit · PostgreSQL · Docker · OpenAI API · Prompt Chaining[cite: 9]
**Rating: 8.7/10**[cite: 9]

- Production-grade automated Text-to-SQL pipeline and state-based FastAPI SQL Agent over `classicmodels` PostgreSQL database[cite: 9]
- Modular agent workflow: Planner → Generator → Validator → Executor → Summarizer with self-correction (up to 3 retries)[cite: 9]
- Vanilla Python prompt-chaining with GPT-4o-mini, rule-based SQL safety validation (blocking DML/DDL), structured JSON query logging[cite: 9]
- **100.0% execution success rate and 100.0% result accuracy** on 50-question benchmark, zero retries required[cite: 9]
- Streamlit chat interface + Docker/Docker Compose containerization[cite: 9]
- GitHub: `AaradhyaDT/fuseAiF_wk3_text2sql`[cite: 9]

### 3. Telco Customer Churn & CLV Machine Learning Pipeline (Fusemachines Week 4) *(Completed)*
**Stack:** Python · Scikit-learn · Pandas · NumPy · Matplotlib · Seaborn · Papermill[cite: 9]
**Rating: 8.5/10**[cite: 9]

- End-to-end classification + regression pipeline for Telco Churn and CLV modeling[cite: 9]
- Stratified 70/15/15 split; Logistic Regression / Ridge / SGD classifiers benchmarked[cite: 9]
- Custom threshold at 0.385 → top-200 high-risk budget segment[cite: 9]
- Ridge Regression best for CLV (mean CLV $1,304.70); Lasso L1 regularization paths plotted[cite: 9]
- Stratified 5-fold CV: ROC-AUC 0.841 ± 0.005; learning curves + leakage simulation[cite: 9]
- Papermill automation; full HTML report export; Graphify knowledge graph integration[cite: 9]
- GitHub: `AaradhyaDT/FUSE_AIF_2026_M1` (under `WK4/`)[cite: 9]

### 4. Telco Churn Tree-Based Ensemble Pipeline (Fusemachines Week 5) *(Completed)*
**Stack:** Python · Scikit-learn · XGBoost · imbalanced-learn · SHAP · Joblib · Matplotlib[cite: 9]
**Rating: 9.0/10**[cite: 9]

- End-to-end classification pipeline on Telco Customer Churn (7,043 rows, ~27% positive rate, binary target)[cite: 9]
- Models: Random Forest + XGBoost benchmarked against naïve baseline; AUROC, Precision, Recall, F1 as primary metrics (accuracy trap exposed)[cite: 9]
- Full Scikit-learn `ColumnTransformer` pipeline for mixed dtypes (numeric scaling + categorical encoding); `ImbPipeline` (imbalanced-learn) ensures SMOTE restricted to training folds only — zero preprocessing leakage[cite: 9]
- Hyperparameter tuning via Grid Search / Bayesian optimisation on XGBoost; documented most impactful hyperparameter[cite: 9]
- SHAP global summary plot (Q15) + local waterfall/force plot (Q16); 2-sentence retention recommendation for specific at-risk customer[cite: 9]
- Production serialization: full fitted pipeline (ColumnTransformer + SMOTE + model) saved via `joblib` as `telco_churn_pipeline_v1.joblib`[cite: 9]
- Secondary regression task: `tenure` prediction (regression model)[cite: 9]. Defined target and feature matrix, dropped `TotalCharges` leakage column to prevent mathematically defined correlation leakage[cite: 9].
- Trained unconstrained Decision Tree Regressor vs regularized XGBoost Regressor[cite: 9]. Plotted learning curves using 5-fold cross-validation showing overfitting in the unpruned baseline vs generalization in the XGBoost regressor[cite: 9].
- Verified tree model predictions are strictly bounded by the training range maximums (extrapolation check)[cite: 9].
- Model Card (Q18) completed with real metric values[cite: 9]
- GitHub: `AaradhyaDT/fuseAiF_wk5_telco_churn_ensembles`[cite: 9]

### 5. Alpha Android Super-App *(Active)*
**Stack:** Kotlin · Jetpack Compose · Material3 · DataStore · Apache POI[cite: 9]
**Rating: 8.2/10 — Primary shipping target**[cite: 9]

- Modular super-app (`com.alpha`, SDK 36, Astronomus font)[cite: 9]
- Modules: SBR gesture control (MediaPipe, CameraX, HC-05 BT) · Multi-mode calculator (STD / PROG / LOGIC) · Settings (DataStore) · Budget Tracker (eSewa parser, Apache POI, DataStore persistence — Google Drive backup in progress)[cite: 9]
- Location: `D:\Android\Projects`[cite: 9]

### 6. Edge AI Stability Detection System *(Completed)*
**Stack:** Python · Scikit-learn · FastAPI · Joblib[cite: 9]
**Rating: 7.8/10**[cite: 9]

- ML system predicting platform stability from simulated IMU sensor data (tilt_x, tilt_y, angular velocity)[cite: 9]
- 10,000-sample synthetic dataset; Random Forest classifier — **99.8% test accuracy**[cite: 9]
- REST API via FastAPI for real-time predictions; Joblib export for robotics integration[cite: 9]
- GitHub: `AaradhyaDT/stability-ai-system`[cite: 9]

### 7. SysOptimizer — Windows Optimization Tool *(v5 Active)*
**Stack:** Python · CustomTkinter · PyInstaller · WMI · PowerShell[cite: 9]
**Rating: 7.6/10**[cite: 9]

- Standalone `.exe` via PyInstaller; animated ring gauges, sparklines, process table, dark/light mode[cite: 9]
- v5: Stricter RAM reclamation, CPU boost clock fix via WMI, Background Bloat & Startup Apps overhaul[cite: 9]
- `CREATE_NO_WINDOW` creationflags — zero UI interruption[cite: 9]

### 8. Major Project — PrakopNet *(Idea D — CONFIRMED PRIMARY, June 8, 2026)*

**Full title:** PrakopNet: A Solar-Powered LoRa Mesh Multi-Hazard Early Warning System with Federated Edge AI for Nepal's Disaster-Prone Regions

**Team:** Aaradhya Dev Tamrakar · Rupesh Kadel · Sankalpa Lamsal · Sonia Thapa (KEC BEI Batch 2081)

**Status as of June 24, 2026:**
Idea D (PrakopNet) is the confirmed major project direction. Idea C (Counter-UAV) has been archived. **Proposal deadline: July 2, 2026.** **Demo deadline: March 2027 (8th semester boards).** Supervisor not yet assigned — group formation for 8th semester is different from last year; pending KEC assignment. Holiday alignment meeting held June 24, 2026 to freeze scope, confirm roles, and draft proposal content. `PrakopNet_MASTER_v0_20260624.md` generated as operative project truth post-session.

**External Advisory Integration (Umesh/HPCNepal — June 2026 Friday session):**
- **Animal behavior precursor signals (de-scoped):** Tracking unusual biological movements requires acoustic classifiers or camera vision nodes — scope trap for a 6-month build. Confirmed de-scoped June 24. Documents only in **Chapter 6: Future Work** of the thesis as "Phase 2 Bio-sensing expansion." Do not include in proposal or active BOM.
- **ICIMOD Data Partnership (green-lit):** ICIMOD's Regional Information Management System (RIMS) confirmed as primary data source alongside DHM. Provides historical landslide inventories, GLOF datasets, and precipitation records for LSTM pre-training. List explicitly in proposal methodology as "data partnerships with DHM and ICIMOD."

**Software Design Patterns (OOSE — added June 24, 2026):**
- **Factory Pattern (Edge Nodes):** `SensorNode` abstract base class → concrete `HydrologicalNode` (Module A) and `GeologicalNode` (Module B). Base handles LoRa TX, deep-sleep, health check, INA219 logging. Enables clean modular expansion.
- **Observer Pattern (Alert Ecosystem):** Gateway is Subject (HazardScore state holder). Observers: Streamlit dashboard, Telegram Bot, Twilio SMS. State update auto-notifies all observers.

**Work Packages (WBS — formalised June 24, 2026):**
| WP | Owner | Core Deliverables | July 2026 Benchmark |
|---|---|---|---|
| WP 1.0 — AI & Data | **Aaradhya** | TFLite Micro edge models · Gateway LSTM · HazardScore fusion · FastAPI/Docker · LaTeX thesis | FastAPI gateway container running locally; ICIMOD data downloaded |
| WP 2.0 — Firmware & Mesh | **Rupesh** | ESP32 C++/Arduino firmware · LoRa mesh routing + app-layer ACKs · Deep-sleep optimization | Stable UART AT-command exchange with RYLR890 via CP2102 + laptop |
| WP 3.0 — Hardware & Power | **Sankalpa** | Circuit integration · CN3791 solar · 18650 testing · IP65 enclosure CAD (Makerspace) | CN3791 thermal + efficiency benchmark with 18650 cells |
| WP 4.0 — UI & Alerting | **Sonia** | Streamlit dashboard · GPS map · Telegram/SMS alerts · Overleaf proposal layout | Streamlit frontend rendering mock JSON payloads |

**Note on Sonia's Overleaf scope:** She owns proposal Overleaf layout (formatting, diagrams, risk matrix, Gantt). Ongoing thesis LaTeX remains Aaradhya's primary.

**HazardScore Fusion Equation (refined June 24, 2026):**
`HazardScore = w_f·(ΔD/Δt) + w_l·(Δθ/Δt)`
Where D = ultrasonic distance (water level, Module A), θ = tri-axial tilt angle (slope displacement, Module B), w_f and w_l = dynamically scaled empirical weight coefficients from ICIMOD historical terrain thresholds.

**Module C Scope Status (unresolved — decide June 24 meeting):**
Phase 5 reinstated Module C (air quality: MQ135 + PMS5003). Gemini Phase 6 deleted it for proposal clarity (dual-hazard only). Decision pending. Recommended disposition: keep in BOM and procurement (PMS5003 already in import-first list), frame as supplementary data layer in proposal — not primary novelty claim.

**Star vs Mesh Topology (unresolved — Rupesh to own call, decide before August):**
6-month build window (Sep 2026 → Mar 2027). Full-scope viable at core level (80% confidence); full scope including all 🟠–🟢 items is 50% confidence — scope-lock at project kickoff is essential. Order all import components in Month 1 (2–3 week AliExpress/Amazon India lead time). All LoRa modules are now import-only (see LoRa compliance note below).

**LoRa Frequency Compliance (confirmed June 10, 2026):**
Nepal legal band: **865–867 MHz** (IN865-867 channel plan, NTA). Max 1W TX / 4W ERP. The 433 MHz band (EU433) is legal but limited to 10 mW ERP — insufficient for the 3–15 km range claims. US915/AU915 (902–928 MHz) is **illegal** in Nepal (assigned to Ncell/NTC 4G).

**Critical BOM change (June 10, 2026):**
LoRa RA-02 (SX1276, 410–525 MHz / 433 MHz variant) **removed** from BOM — 433 MHz ERP limit invalidates range claims. Replaced with **RYLR890 (868 MHz, UART AT commands)**. Also: HC-SR04 → JSN-SR04T (waterproof); TP4056 → CN3791 (solar-rated charge controller); INA219 current sensor added (power budget measurement, thesis contribution).

**Nepal hardware availability (updated June 10, 2026):**
| Component | Source | Availability |
|---|---|---|
| ESP32-WROOM-32 (DevKit V1) | Himalayan Solution, Breadfruit | ✅ Local, same-day |
| RYLR890 (LoRa 868 MHz, UART) | Import — AliExpress / Amazon IN | ⚠️ **Order Month 1; specify 868 MHz** |
| Neo-6M GPS | Himalayan Solution | ✅ Local |
| MPU6050 | Himalayan Solution, Breadfruit | ✅ Local |
| DHT22 | Himalayan Solution, Breadfruit, Daraz | ✅ Local |
| JSN-SR04T (waterproof ultrasonic) | Import | ⚠️ Order Month 1 — not HC-SR04 |
| Capacitive soil moisture sensor | Himalayan Solution, Breadfruit | ✅ Local |
| MQ135 (air quality) | Himalayan Solution, Breadfruit | ✅ Local |
| PMS5003 (PM2.5) | Import | ⚠️ Order Month 1 (2–3 wk lead) |
| 6V 5W solar panel | Local electronics, Daraz | ✅ Local |
| CN3791 solar charge controller | Import / Daraz | ⚠️ Order Month 1 |
| 18650 Li-ion (protected, 3000–3500 mAh) | Local battery shops, Daraz | ✅ Local |
| MT3608 boost converter | Himalayan Solution, Breadfruit | ✅ Local |
| INA219 current sensor | Import / Daraz | ⚠️ Order Month 1 |
| Raspberry Pi 4B (4GB) | Breadfruit (inconsistent stock) | ⚠️ Check early; import from Amazon IN if OOS |
| Weatherproof enclosures | 3D print (KEC Makerspace) | ✅ Makerspace |

**Fusemachines fellowship → PrakopNet skill mapping (confirmed June 10, 2026):**
| Fellowship Output | PrakopNet Role |
|---|---|
| LSTM (Wk4 CLV time-series) | Core edge inference: sensor time-series → hazard score |
| SMOTE (Wk5) | Imbalanced disaster event data — same fix |
| SHAP (Wk5) | Explainability for defense: which sensor triggered alert |
| XGBoost/RF (Wk5) | Lightweight fallback classifier on gateway |
| FastAPI + Docker (Wk3) | Base station dashboard + alert API |
| Papermill (Wk4) | Automated retraining pipeline on new seasonal data |
| PC-side pipeline discipline | Training → TFLite quantization → ESP32 deployment chain |

**Team ownership (locked — see team split table above):**
- Firmware/hardware node + LoRa mesh + gateway hardware: **Rupesh** (primary) + **Sankalpa** (hardware assembly, solar, 3D design)
- ML pipeline (training → quantize → TFLite deploy) + HazardScore fusion + LaTeX thesis: **Aaradhya**
- Backend (FastAPI) + grant writing: **Aaradhya** (secondary)
- Dashboard frontend (Streamlit/Flask) + data logging + GPS visualization: **Sonia** (primary)
- Report/documentation co-lead (thesis structure, section drafts): **Sonia** (secondary)

**Architecture:**
- **Sensor Nodes:** ESP32 DevKit V1 + RYLR890 (LoRa 868 MHz, UART AT commands) + GPS (Neo-6M) + Solar subsystem (6V 5W panel → CN3791 charge controller → 18650 ×2 parallel → MT3608 boost → 5V) + INA219 power monitor + environmental sensors
- **Gateway:** Raspberry Pi 4B (4GB RAM) + RYLR890 (UART) + dashboard server + PostgreSQL + AI processing
- **AI Layer:** Federated TFLite Micro on ESP32 nodes (local binary anomaly decision) + LSTM at gateway (multi-sensor time-series → HazardScore) + TFLite runtime at gateway

**Modular Sensor Modules:**
- Module A — Flood: ultrasonic water level sensor
- Module B — Landslide: MPU6050 + optional geophone
- Module C — Air Quality: MQ135 + PM2.5
- Module D — Weather: rain gauge, wind, humidity
- Module E — Wildfire: smoke + temperature
- Module F — Structural Health: strain gauges, vibration sensors

**Build Phases:**
- Phase 1: ESP32 + LoRa + GPS + MPU6050 + DHT22 + solar subsystem → basic network
- Phase 2: Water level + rainfall monitoring
- Phase 3: Geophone + GSM backup + PM2.5

**Assessment:**
| Dimension | Current | Target |
|---|---|---|
| Academic Value | 9/10 | 9.5/10 |
| Commercial Potential | 9/10 | 9.5/10 |
| Buildability | 9/10 | 9/10 (hold) |
| Research Novelty | 7.5/10 | 8.5–9/10 |
| Nepal Relevance | 10/10 | 10/10 (hold) |

**What's locked — do not touch:**
ESP32 + LoRa SX1278 + Neo-6M GPS + Solar + 18650 per node · RPi 4B as gateway · LoRa mesh topology · LSTM + TinyML at AI layer · Module A (Flood) + Module B (Landslide) as core two · MPU6050 for seismic · DHT22 for temperature/humidity

**Phase 5 Technical Modifications (originally from HimalGuard_Modifications_v1, now in MASTER_MajorProject_ChronologicalMerge_v2):**

| Modification | Priority | Build Effort | Impact |
|---|---|---|---|
| **Federated TFLite edge inference on ESP32 nodes** — each node runs local binary anomaly model; alerts fire even if LoRa gateway link degraded; direct transfer from GCSBR + Edge AI Stability Detection work | 🔴 1 — Do not drop | 2–3 weeks | Novelty +1 point; disaster resilience |
| **Multi-hazard composite HazardScore (0–100)** — gateway fuses WaterLevel + SeismicAmplitude + RainfallRate + SlopeInstability with tunable weights per zone; threshold bands Green/Amber/Red | 🟠 4 | 1 week | Novelty +0.5; commercial clarity |
| **Solar power telemetry logging** — ADC voltage read on ESP32 → log panel voltage + battery SoC per node per interval; publishable empirical dataset (no Nepal equivalent exists) | 🟠 5 | 2–3 hrs HW + 1 day firmware | New empirical contribution |
| **Adaptive LoRa Spreading Factor** — nodes auto-select SF7–SF12 based on RSSI from last gateway ACK; graceful degradation in disaster conditions | 🟡 6 | 1 week | Disaster robustness |
| **GPS-fenced alert zones** — lat/lon polygon per deployment zone; alert propagates only if anomaly falls within boundary | 🟡 7 | 2–3 hrs (point-in-polygon) | Reduced false positives; commercial pitch strength |

**Scope cuts:**
- Modules E (Wildfire) and F (Structural Health) → document as future work
- Geophone → MPU6050 covers the need; document as upgrade option
- GSM backup → LoRa mesh handles graceful degradation; document as future work
- >3 physical nodes → build 2–3 real; simulate mesh scale in thesis
- Module C (Air Quality): MQ135 + PM2.5 ✅ (viable with 6-month timeline — procure early September)
- Module D (Weather): DHT22 + one rain sensor only

**Research novelty fix strategy (7.5 → 8.5+):**
1. **Literature gap statement (Chapter 1):** "Existing LoRa-based EWS address single-hazard monitoring in isolation. No published system demonstrates multi-hazard fusion with edge-computed composite risk scoring, GPS-tagged anomaly localization, distributed ESP32 TFLite inference, and solar-powered autonomous mesh operation validated in South Asian deployment contexts." Each clause independently verifiable on IEEE Xplore.
2. **Real sensor data for LSTM:** Deploy ≥1 node for 2–4 weeks before thesis submission (Oct–Nov 2026). Even 2 weeks of clean time-series is sufficient for anomaly threshold calibration. Real-data LSTM = a result; synthetic LSTM = background method.
3. **Measured power budget as standalone contribution:** Current draw at deep sleep / sensor active / LoRa TX (measure with multimeter); panel output hourly log; battery endurance calculated + measured → "Node X operates autonomously for Y days on Z mAh at Nepal average irradiance."

**Makerspace deliverables:**
- 3D printing: weatherproof node enclosures (IP54+ minimum) — separate compartments for battery, sensor, electronics; cable glands; solar panel mounting tab; snap-fit lid with gasket channel. Gateway housing (RPi 4B + LoRa hat, vented semi-outdoor).
- Laser cutting: pole/fence mounting bracket for field deployment; internal node chassis to fix sensor positions (reduces MPU6050 mechanical noise); acrylic gateway display panel.
- 1Gbps WiFi: full Docker stack (PostgreSQL + FastAPI + Streamlit) locally; real-time data streaming tests; heavy LSTM training without bandwidth constraint.

**Commercialization pathway:**
Build for academic submission: Basic Tier (live sensor feed, alert status, GPS map markers).
Document as product roadmap (Chapter 6): Professional Tier (LSTM predictions, historical analytics, PDF report export) · Enterprise Tier (GIS polygon overlays, multi-site management, API for municipalities).
One real client conversation before graduation — target one municipality ward office, one local NGO (Red Cross Nepal), or one hydropower project. Even informal letter of interest = grant applications 10× stronger.
PrakopNet landing page: 2–3 hours on portfolio stack; host on GitHub Pages; use as Makerspace Ambassador web dev deliverable.
Grant applications (submit Oct 2026): UNDP Nepal Innovation Challenge · NRCS innovation calls · Social Alpha · Rockefeller ACCRN.

**8th Semester Execution Timeline (Sep 2026 → Mar 2027):**
| Month | Phase | Deliverables |
|---|---|---|
| September | Core hardware build | 2 nodes assembled + LoRa link established + gateway running + basic dashboard live |
| October | Intelligence layer | LSTM at gateway + TFLite micro on nodes + HazardScore fusion + solar telemetry logging + early node deployment (real data begins) |
| November | Polish + field test | 3D printed enclosures (Makerspace) + 1 outdoor field deployment + GPS-fenced zones + adaptive SF + Module C (MQ135 + PM2.5) |
| December | Documentation | LaTeX thesis drafting + dashboard UI final + grant applications submitted + landing page live |
| January | Thesis writing | LaTeX full draft (Ch 1–6) + measured power budget documented + LSTM retrained on real data |
| February | Revision + demo prep | Supervisor feedback incorporated + demo script + system stress-tested |
| March | Submission | Thesis submitted + demo ready for boards |

**Rule:** Each month has one deliverable that must work before next month starts. No month N+1 work begins until month N deliverable is demonstrated.

**Team role split (8th semester — locked):**
| Member | Primary | Secondary |
|---|---|---|
| **Aaradhya** | TFLite micro (ESP32 nodes) + LSTM training (gateway) + HazardScore fusion + LaTeX thesis | Dashboard backend + grant writing |
| **Rupesh** | LoRa mesh firmware + RF link budget analysis + adaptive SF + gateway hardware | Solar telemetry firmware |
| **Sankalpa** | Hardware assembly + sensor integration + solar subsystem + 3D model design (Makerspace) | GPS firmware |
| **Sonia** | Dashboard frontend (Streamlit/Flask) + data logging + GPS map visualization | Documentation + testing |

**Modification priority stack:**
🔴 1 — Federated TFLite inference (no drop) · 🔴 2 — Real sensor data for LSTM (no drop) · 🔴 3 — 3D printed weatherproof enclosures (no drop) · 🟠 4 — HazardScore fusion (drop → future work) · 🟠 5 — Solar telemetry dataset (drop → secondary) · 🟡 6 — Adaptive LoRa SF · 🟡 7 — GPS-fenced zones · 🟢 8 — PrakopNet landing page (fast, 2–3 hrs) · 🟢 9 — Grant applications (submit ≥1)

**Key documents:**
- `PrakopNet_MASTER_v0_20260624.md` — **current operative project truth** (supersedes all ChronologicalMerge docs)
- `MASTER_MajorProject_ChronologicalMerge_v4_UPDATED.md` — superseded by PrakopNet_MASTER_v0
- `TEAM_PROFILE_SYSTEM_v17_20260610.md` — team profiles (TBDs pending June 24 resolution)
- `gemini_phase_6_.md` — absorbed into PrakopNet_MASTER_v0

**Archived — Idea C (Distributed TinyML Counter-UAV):**
Was primary at ~85% confidence as of June 2, 2026. Architecture: RTL-SDR + RPi 4B → ESP32 + INMP441 TFLite acoustic nodes → ESP32-CAM YOLO-nano → LoRa alert mesh → Flask + SQLite + Android. Archived in favour of PrakopNet due to stronger commercial/completion profile. Full spec in IDEATION_MasterConsolidated_v3.

### 9. Custom Processor FSM Design *(Completed — Coursework)*
**Stack:** VHDL · Vivado 2023.2[cite: 9]
**Rating: 6.8/10**[cite: 9]

- VHDL implementation of a custom processor datapath and FSM for GCD and exponentiation operations[cite: 9]
- Simulated and verified in Vivado 2023.2 (Embedded Systems coursework)[cite: 9]

### 10. Fusemachines AI Fellowship Prep Toolkit *(Completed)*[cite: 9]
- 50-question mock exam widget + 7-tab interactive HTML cheatsheet (linear algebra, calculus, probability, Python/CS, ML)[cite: 9]

### 11. Fusemachines Week 6 Probabilistic Models Assignment *(Completed)*
**Stack:** Python · PyMC · ArviZ · pgmpy · scikit-learn · Pandas · Matplotlib · Seaborn[cite: 9]

- Week 6 repository structure confirmed: `W6_Probabilistic_Models_Assignment.ipynb`, `W6_TaskPlan.md`, `TASK_PROGRESS.md`, and `W6_Probabilistic_Models_Resource_Guide.pdf`.
- Core deliverables: Bayesian estimation (MLE/MAP/full Bayes), sequential updating, Dirichlet-multinomial inference, multivariate Gaussian conditioning, probabilistic graphical models, Gaussian process regression, and PyMC Bayesian logistic regression.
- Artifact saved: `telco_bayes_lr_v1.pkl` from the Bayesian logistic regression trace.
- Portfolio entry live on `aaradhyadtmr.github.io` under Projects.

### 12. Fusemachines Week 7 Clustering Assignment *(Completed — June 12, 2026)*
**Stack:** Python · scikit-learn · scipy · Pandas · NumPy · Matplotlib · Seaborn · NearestNeighbors
**Dataset:** UCI Online Retail II (~500,000 transactions, `Year 2010-2011` sheet)
**Repo:** `AaradhyaDT/fuseAiF_wk7_customer_segmentation`

- **Context:** Market segmentation — build customer profiles from raw transaction data with no labels.
- **Pipeline:** Raw transactions → RFM feature engineering + extended features (AvgBasketSize, AvgDaysBetweenPurchases, UniqueProducts, ReturnRate) + **category spend ratios** (keyword-bucketing on `Description` into ≥5 categories: Gift/Home/Seasonal/Stationery/Other) → preprocessing (IQR + Z-score outlier detection compared; StandardScaler vs RobustScaler explicit decision) → K-Means (Elbow + Silhouette, k-means++ vs random init comparison) → Hierarchical (Ward + Complete + Average + Single dendrograms; fit Ward + Complete) → DBSCAN (k-distance ε estimation, ≥3 param combos, noise analysis) → validation (Silhouette / Davies-Bouldin / Calinski-Harabasz) → business narrative (cluster profiles + executive summary) → failure log (≥3 entries).
- **Status:** Notebook executed end-to-end, all sections S0–S9 complete; submitted as `Week_7_Clustering_Assignment_executed.ipynb`. Repo organized — root contains executed notebook, assignment PDF, plots/, README, LICENSE, .gitignore (raw `.xlsx` dataset gitignored); dev artifacts/debug scripts/task plans archived under `misc/`.
- **Submission:** Single `.ipynb`, all cells executed, handed in via Google Classroom (AI Fellowship 2026) — due June 21, 2026.

> ~~**PORTFOLIO TRIGGER:** Week 7 Clustering Assignment~~ — ✅ Entry live in shipped `projects.html` (v113). Trigger resolved.

### 13. RF and Microwave Engineering Lab Reports *(Active — June 2026)*
**Tool:** Keysight ADS (Advanced Design System) · LaTeX (KEC report template)

- **Lab 1 — Introduction to ADS** *(Complete)*: DC sweep (voltage divider), AC analysis (series RLC S-parameters, resonance ~300 MHz), parameter sweep (RC circuit, capacitance 1–10 pF). Report `lab_report_ADS_Lab1.pdf`.
- **Lab 2 — Impedance Matching Networks** *(Complete)*: (1) Quarter-wave transformer matching 50Ω source to 150Ω load at 100 MHz — design $Z_0'=86.25\,\Omega$ vs. theoretical $\sqrt{50\times150}=86.60\,\Omega$, return loss $-47.8$ dB at 100 MHz. (2) Lumped L-section match for $15+j10\,\Omega$ load to 50Ω at 2.5 GHz via ADS Smith Chart Matching Utility (shunt C + series L); first iteration $-55.5$ dB, refined values ($C=1.945$ pF, $L=822$ pH) achieved $-134.3$ dB — verified analytically. Report `lab_report_ADS_Lab2.pdf` + `.tex` source.

### 14. Antenna Lab Data Analysis[cite: 9]
- Python script for antenna radiation pattern from Excel[cite: 9]. Pandas, NumPy, Matplotlib (polar), SciPy (cubic interpolation)[cite: 9].

### 15. Nexus — Personal AI Operating System *(Active — T13+T14 done June 13, 2026)*
**Stack:** React (Vite) · FastAPI · SQLite + FTS5 · httpx · asyncio
**Repo:** `AaradhyaDT/nexus` · **License:** MIT

> **TRIGGER:** When "Nexus" is mentioned, load this full context before responding.

**Vision:** Not a chatbot. A project-centric AI operating system that unifies Groq (Llama 3.3 70B) and Gemini into one workspace — replacing the multi-browser, multi-account, multi-tool fragmented workflow.

**Core concept:** One prompt → one project context → multiple model outputs (parallel fan-out) → centralized persistent memory.

**Architecture (v2 — confirmed June 12, 2026):**
```
React Frontend (localhost:5173)
        ↓ REST
FastAPI Backend (localhost:8000)
        ↓
   SQLite — nexus.db
   ├── projects  (name, g_index, g_email, system prompt)
   ├── history   (prompt, responses JSON, models_used, timestamp)
   └── FTS5      (project_notes_fts — auto context injection)
        ↓
   Model Router
Groq (Llama 3.3 70B) · Gemini 2.5 Flash
```

**v2 key decisions:**
- **SQLite replaces PostgreSQL** — single `nexus.db` file, no service to run, `contextmanager` pattern
- **FTS5 replaces ChromaDB** — native SQLite full-text search; relevant notes auto-prepended to system prompt on every query; zero embedding latency
- **No OAuth storage** — Google account routing via index-swap (`/u/0`, `/u/1`); project stores `g_index` + `g_email` label only; browser sessions handle auth
- **Single `main.py`** — all routes, adapters, DB, FTS injection in one file (~130 lines)
- **Multi-key rotation** — comma-separated `GROQ_API_KEYS` / `GEMINI_API_KEYS` pools; auto-retry on 429/401/403

**Task plan:** `Plan/Nexus_MasterPlan_v2.md` — 24 tasks across 4 phases (canonical, supersedes all Day 1/Day 2/Complete_TaskPlan docs).

**MVP scope (v0.2 → v0.5 → v1.0):**
| Feature | Status |
|---|---|
| Project workspaces (create/switch) | ✅ |
| Multi-model parallel fan-out (Groq + Gemini) | ✅ |
| Side-by-side results, dynamic columns | ✅ |
| Persistent history — SQLite | ✅ |
| FTS5 context injection from project notes | ✅ |
| Google account index routing (sidebar links) | ✅ |
| Multi-key rotation | ✅ |
| Dark/light theme toggle | ✅ |
| Clear history (backend DELETE route + UI) | ✅ |
| Gemini 2.5 Flash live confirmed | ✅ |
| Notes UI (save/view/delete from frontend) | ✅ T13 done June 13 |
| Project system prompt editor (Settings modal) | ✅ T14 done June 13 |
| Markdown rendering (zero-dep `renderMarkdown()`) | ✅ T13/T14 session |
| start-nexus.bat cold launch verified | ⬜ Phase 3 |
| History deletion DB-level verified | ⬜ Phase 3 |
| Cost/token tracker | ⬜ v0.5 T15 |
| History search + Markdown export | ⬜ v0.5 T16/T17 |
| Ollama local model support | ⬜ v1.0 |
| Task-aware routing | ⬜ v1.0 |
| Agent mode | ⬜ v1.0 |

**Build log:**
- **Day 1 (June 10, 2026):** Backend skeleton — Groq + Gemini fan-out via `asyncio.gather`, multi-key rotation, CORS. Frontend — Vite React, textarea, side-by-side results. End-to-end confirmed ✅
- **Day 2 (June 11–12, 2026):** Architecture pivoted from PostgreSQL+ChromaDB to SQLite+FTS5 (v2). Full backend rewrite. Full frontend redesign — dark editorial UI, project sidebar, Google account routing, history panel. v2 complete ✅. UI verified rendering correctly (design/sidebar/forms ✅; model pills require backend running). Folder structure corrected (backend/, frontend/src/ — was flat) ✅
- **Day 3 (June 13, 2026):** Gemini 2.5 Flash live-confirmed ✅. Both models (Groq + Gemini) verified responding in parallel. `MasterPlan_v2.md` generated — 24 tasks, 4 phases, supersedes all prior plan docs. Pending: start-nexus.bat cold launch, history deletion DB-level check, theme persistence verify.
- **Day 4 (June 13, 2026, afternoon):** T13 Notes UI ✅ + T14 Project system prompt editor ✅ — both implemented and confirmed working (screenshot 2:10 PM). Backend additions: `GET /projects/{id}/notes`, `DELETE /projects/{id}/notes/{note_id}`, `PATCH /projects/{id}` (supports name/prompt/g_index/g_email partial update). Frontend: collapsible notes panel (textarea + Save note + per-note × delete + note count badge + "Note saved" toast); Settings text button (replaces ⚙ glyph — cross-platform rendering fix); settings modal (system prompt textarea, g_email, g_index, PATCH on save, "Saved" toast, backdrop dismiss). Markdown rendering added: zero-dep `renderMarkdown()` (~80 lines) handles **bold**, *italic*, `` `code` ``, fenced code blocks with lang label, h1/h2/h3, ul/ol, `---` hr, blank lines → `<br>`, paragraphs; output columns now use `nx-md-body` div (wrapping prose) instead of `<pre>`. Both Groq and Gemini responses render formatted markdown ✅.

**Key risks:**
| Risk | Mitigation |
|---|---|
| API cost blowup from fan-out | Token tracker per project (v0.5 T15) |
| Context window overflow in long sessions | Summarization layer — don't raw-append history |
| Completion gap | Treat each session like a Fellowship deadline |

**Portfolio angle:**
- Benchmark: show parallel routing improves output quality vs. single-model baseline
- Technical writeup: "Multi-model orchestration with FTS5 context injection"
- MCP integration (v1.0) signals agentic tool standard awareness

**Strategic note:** Nexus is also PrakopNet's development infrastructure. The project notes + FTS5 layer = same architecture needed for sensor logs, LSTM experiment records, and literature references.

---

## 🏅 Project Ranking (v5 — May 2026)

| Rank | Project | Score | Status |
|------|---------|-------|--------|
| 1 | GCSBR | 9.4 | Complete[cite: 9] |
| 2 | Telco Churn Tree-Based Ensemble Pipeline (Wk5) | 9.0 | Complete[cite: 9] |
| 3 | Text-to-SQL Agentic Pipeline (Wk3) | 8.7 | Complete[cite: 9] |
| 4 | Telco Churn & CLV Pipeline (Wk4) | 8.5 | Complete[cite: 9] |
| 5 | Fusemachines Week 6 Probabilistic Models Assignment | 8.2 | Complete — portfolio entry live |
| 6 | Alpha Android Super-App | 8.2 | Active[cite: 9] |
| 7 | Edge AI Stability Detection System | 7.8 | Complete[cite: 9] |
| 8 | SysOptimizer | 7.6 | v5 Active[cite: 9] |
| 9 | Major Project — PrakopNet (Idea D) | 7.5→8.5+ | Confirmed primary (June 8, 2026); Phase 5 modifications integrated; novelty target 8.5–9 via federated TFLite nodes + real LSTM data + measured power budget; demo target **March 2027 boards** |
| 10 | Nexus — Personal AI Operating System | 7.0→7.5 | Active — v2 (SQLite+FTS5) complete; both models live June 13, 2026; T13 Notes UI + T14 Settings modal done June 13, 2026; markdown rendering live; MasterPlan_v2 (24 tasks) in progress |
| 11 | Fusemachines Week 7 Clustering Assignment | 8.0 | Complete — June 12, 2026; submitted; portfolio entry live in `projects.html` (v113) |
| 12 | Custom Processor FSM Design | 6.8 | Complete[cite: 9] |
| 13 | Fuse Fellowship Prep Toolkit | 6.5 | Complete[cite: 9] |
| 14 | Antenna Lab Data Analysis | 5.2 | Complete[cite: 9] |
| 15 | RF and Microwave Engineering Lab Reports | 5.5 | Active — Lab 1 & Lab 2 complete (June 13, 2026) |

**Completion is the ceiling limiter[cite: 9]. Alpha on Play Store or Major Project demo would be the single highest-leverage next ship[cite: 9].**

---

## 🔧 Fellowship Dev Standards — 12-Factor Pre-Commit Checklist (§16)

> **Rule:** Run this checklist at least once before every final `git commit` on any Fusemachines fellowship repo or Nexus. Not optional. Not "if I remember." Before the commit.

The [12-Factor App](https://12factor.net) methodology defines production-grade software. For fellowship repos, this maps to: code that a reviewer can run cold, reproduces results exactly, and doesn't fail because of a missing env var or hardcoded path.

### The 12 Factors — Pre-Commit Verification

| # | Factor | What to check before commit |
|---|--------|----------------------------|
| **1** | **Codebase** | One repo per project. No untracked experiment branches floating locally. `git status` clean except intentional staged files. |
| **2** | **Dependencies** | `requirements.txt` / `pyproject.toml` / `package.json` updated and pinned. No implicit `pip install X` in README that isn't in the lockfile. Run `pip install -r requirements.txt` in a clean venv to verify. |
| **3** | **Config** | Zero hardcoded secrets, API keys, DB passwords, or absolute paths in code. All config via `.env` (not committed). `.env.example` committed with placeholder values. `.env` in `.gitignore`. |
| **4** | **Backing services** | DB connection strings, external APIs, storage paths all read from env vars — not hardcoded. Swapping Postgres → SQLite should require only a `.env` change. |
| **5** | **Build / Release / Run** | Dockerfile (if present) separates install from runtime. No `pip install` in the `CMD`/entrypoint. Build artifacts not committed (`.gitignore` covers `__pycache__/`, `*.pyc`, `dist/`, `.venv/`). |
| **6** | **Processes** | App is stateless between requests. Session state goes in DB / cache, not in-memory global variables. Verify no module-level mutable state that breaks if two workers run. |
| **7** | **Port binding** | App binds to a port from env var (`PORT` / `BACKEND_PORT`). No hardcoded `8000` or `3000` in code — only in `.env.example`. |
| **8** | **Concurrency** | If using `asyncio.gather` (Nexus fan-out) or Papermill parallel runs — confirm no shared mutable state between concurrent tasks. Worker count set via config, not hardcoded. |
| **9** | **Disposability** | App starts fast (< 5s cold). Graceful shutdown handles SIGTERM (FastAPI lifespan / `finally` blocks). No orphaned DB connections on crash. |
| **10** | **Dev/prod parity** | `docker-compose.yml` (if present) mirrors prod stack exactly. Python version in `runtime.txt` / Dockerfile matches local. No "works on my machine" hacks committed. |
| **11** | **Logs** | No `print()` debug statements left in committed code. Use `logging` module with level controlled by env var (`LOG_LEVEL=INFO`). Logs go to stdout (captured by Docker / systemd). No log files committed. |
| **12** | **Admin processes** | DB migrations, seed scripts, one-off data fixes — all in standalone scripts under `scripts/` or `migrations/`. Never baked into app startup. Run once, document in README. |

### Quick Pre-Commit Command Sequence (Fellowship Standard)

```bash
# 1. Check nothing secret is staged
git diff --cached | grep -iE "(api_key|password|secret|token)" && echo "⚠ SECRET DETECTED" || echo "✅ No secrets"

# 2. Verify .env is NOT staged
git diff --cached --name-only | grep "\.env$" && echo "⚠ .env STAGED — remove it" || echo "✅ .env clean"

# 3. Check requirements are updated (Python projects)
pip freeze > /tmp/current_reqs.txt && diff requirements.txt /tmp/current_reqs.txt | head -20

# 4. Run any tests before committing
pytest -q 2>/dev/null || echo "(no tests yet — add at least one smoke test)"

# 5. Final status check
git status && git diff --stat --cached
```

### Per-Repo Compliance Status

| Repo | Factor 2 | Factor 3 | Factor 11 | Notes |
|------|----------|----------|-----------|-------|
| `fuseAiF_wk3_text2sql` | ✅ | ✅ | ✅ | Docker + .env pattern established |
| `fuseAiF_wk5_telco_churn_ensembles` | ✅ | N/A | ✅ | No secrets; notebook-based |
| `fuseAiF_wk7_customer_segmentation` | ✅ | N/A | ✅ | `.xlsx` gitignored ✅ |
| `nexus` | ✅ | ⏳ Check .env.example | ⏳ Replace print() with logging | v2 SQLite+FTS5 — verify before next commit |
| Future fellowship repos | — | — | — | Start from this checklist |

> **Trigger:** This section is the pre-commit gate for all fellowship and Nexus work. Load this section at the start of any dev session where a commit is planned.

### 📝 Instructor Feedback Log

| Week | Feedback | Status |
|---|---|---|
| Wk 2/3/4 (exact week unconfirmed — API project) | **Declutter and organize into subfolders; use separate routers for separate tasks/concerns.** Monolithic single-file API structure flagged — instructor recommended breaking routes into separate router files per domain (e.g. `routers/auth.py`, `routers/query.py`, `routers/results.py`) and keeping a clean folder hierarchy instead of flat project root. Noted in the same session that introduced the 12-Factor App standard (§16, v99) — both are the same code-quality push from the instructor. | ⏳ Not yet applied retroactively — apply to next API-based fellowship project and Nexus |

> **Apply-forward rule:** Any new FastAPI project (fellowship or Nexus) must use `APIRouter` per domain from day one. No monolithic `main.py` with all routes inline. Folder structure: `app/routers/`, `app/models/`, `app/db/`, `app/core/` minimum.

---

## 🌐 Portfolio Website — aaradhyadtmr.github.io

> **STATUS (v113, June 22, 2026):** Multipage migration **complete**. Netlify + Decap CMS is **cancelled** — staying on GitHub Pages. Architecture based on KEC Makerspace codebase patterns (audited June 22, 2026).
>
> **Build progress:**
> | Round | Deliverable | Status |
> |---|---|---|
> | 1 | `assets/css/style.css`, `assets/js/script.js` (shared infra) | ✅ Shipped |
> | 2 | `index.html` (Hero, stats strip, quick-nav cards) | ✅ Shipped (v112) |
> | 3 | `projects.html` (projects grid, 13 cards, tag + link system) | ✅ Shipped (v113) |
> | 4 | `experience.html` (8-item 3-col timeline) | ✅ Shipped (v113) |
> | 5 | `about.html` (bio, photo, skills grid, education, CV link) | ✅ Shipped (v113) |
> | 6 | `contact.html` (EmailJS form + Formspree + mailto fallback) | ✅ Shipped (v113) |
> | + | `sitemap.xml` updated, `README.md` rewritten, `og-image.jpg` 1200×630 | ✅ Shipped (v113) |
> | 7 | `achievements.html` — certificate lightbox (19 cert buttons across 16 items: 13 single + 1 six-cert DataCamp bundle; 2 items with no cert file — IEEE Conference Leadership, Git & GitHub) | ✅ Shipped (v114) — recount verified Jun 25, 2026; NepaTronix Drone cert added since v114, no longer in the "no file" set |
>
> **NOT YET LIVE** — deploy package `aaradhyadtmr_github_io_v7.zip` (22 files) built and verified. Next action: unzip, commit, and push to `AaradhyaDT/AaradhyaDT.github.io` main branch. **Note:** `achievements.html` (v114) not in v7 zip — include separately when pushing.

> **MULTIPAGE BUILD PLAN — GitHub Copilot (Raptor mini) Prompt Sequence**
>
> **Workflow:** Claude writes the scoped prompts; Aaradhya runs them in VS Code Copilot Chat (Raptor mini, Agent/Edit mode). Same orchestration pattern as `makerspace-main`.
>
> **Page structure:**
> - `index.html` — Hero, stats strip, quick-nav cards to other pages
> - `projects.html` — All projects grid (GCSBR, Alpha, Edge AI, Nexus, PrakopNet, Fuse wk6/wk7, Antenna, Custom Processor)
> - `experience.html` — Timeline: IEEE VP, Fuse AI Fellow, DataCamp Fellow, EPC Event Manager
> - `about.html` — Bio, skills stack, education, tools
> - `contact.html` — Email, LinkedIn, GitHub, contact form (EmailJS, already wired)
>
> **Shared infrastructure (build first):**
> 1. `assets/css/style.css` — token system (`:root` / `[data-theme]`), reset, navbar, footer, buttons, cards, section headers. Nothing page-specific.
> 2. `assets/js/script.js` — footer injection (`SITE_FOOTER_HTML` constant + `<div id="siteFooter">`), theme toggle, active nav link detection (`location.pathname.split('/').pop()`), mobile hamburger nav, `SEARCH_INDEX` stub.
> 3. `index.html` first (lightest), then `projects.html`, `experience.html`, `about.html`, `contact.html`.
>
> **Patterns to carry from Makerspace codebase (ranked — memorise these, zip will not be re-uploaded):**
> 1. CSS token system — `:root` / `[data-theme="light"]`, all colors/radius/shadow/transition as vars
> 2. Active nav link — `location.pathname.split('/').pop()` → `.classList.add('active')` on matching `<a>`
> 3. Footer injection — `SITE_FOOTER_HTML` string constant in `script.js`, `<div id="siteFooter">` placeholder in each page
> 4. Shared `script.js` + `style.css` + page-local `<style>` blocks — all page-specific CSS inside `<head><style>` of that page; shared utilities in `style.css`
> 5. Global search — `SEARCH_INDEX` array with `{type, title, desc, href, keywords}` entries; keyword-match filter; results grouped by type
> 6. `.section` / `.section-header` / `.section-label` / `.section-title` / `.section-sub` hierarchy — `clamp()` sizing, uppercase label in `--accent2`
> 7. `.card` with `::before` top-border reveal on hover + `translateY(-3px)` lift — use for project cards
> 8. Button system — `.btn`, `.btn-primary`, `.btn-secondary`, `.btn-outline`, `.btn-lg`
> 9. Navbar — sticky, `backdrop-filter: blur(12px)`, flex single-row (5 links, simpler than Makerspace's 2-row grid)
>
> **What NOT to carry:**
> - Changa One at `font-weight: 700/800` — use at 400 only or swap font; no synthesized bold
> - Footer as 150-line HTML string — keep footer lean (links + socials + copyright only)
> - `fade-in` class that immediately adds `.visible` with no observer — either use real `IntersectionObserver` or drop the class
> - Page-local `<style>` for layout — only for truly page-specific overrides; shared layout goes in `style.css`
> - Inline SVG repeated in every element — use a `<symbol>` sprite or icon font (Lucide/Tabler)
> - 2-row navbar grid (`grid-template-areas: "logo links" / "logo actions"`) — overkill for 5 links; use flex row
>
> **Existing portfolio assets to preserve:**
> - Animation system: `SignalWaveBackground`, revolving arc dividers, double counter-rotating dot rings on status card — migrate to `index.html` only
> - Dark luxury editorial aesthetic: Cormorant Garamond + DM Mono + Instrument Sans — retain as font stack
> - GA4: `G-P38642CDGB` — include in shared `script.js`
> - EmailJS — keep in `contact.html` only
> - `photo.webp` + `photo.png` (`<picture>`) — `about.html`
> - `robots.txt`, `sitemap.xml`, `google3e772e11a3eb8313.html` — repo root, carry forward unchanged; update `sitemap.xml` with new page URLs

- Multipage static HTML/CSS/JS architecture — `index.html`, `projects.html`, `experience.html`, `achievements.html`, `about.html`, `contact.html`, shared `assets/css/style.css` + `assets/js/script.js`[cite: 9]
- **Projects, Experience, Achievements** — hardcoded HTML per page; no CMS layer (Decap CMS + Netlify migration explored June 10, 2026, cancelled at v111)
- **Hosting:** GitHub Pages (static) — see STATUS box above for live/not-live state
- Dark luxury editorial aesthetic: Cormorant Garamond + DM Mono + Instrument Sans[cite: 9]
- Lighthouse/PSI (confirmed live, June 21, 2026, v105): Desktop 99, Mobile 92 (Performance) · Accessibility 100, Best Practices 100, SEO 100 (both)[cite: 9]
- GA4 live: Measurement ID G-P38642CDGB[cite: 9]

### Animation System (as of May 30, 2026)

**Background canvas:** `SignalWaveBackground` — 5 slow sine wave signal traces spanning full viewport, gold/teal accent colours, each with a travelling glowing node. Replaces previous `IsometricHexBackground` (hex grid with mouse proximity shimmer).

**Particle layer:** `SparkSystem` (floating embers + click burst) — **removed**. `#particle-canvas` hidden.

**Dividers:** Revolving arc style (CW accent sweep + CCW accent2 counter-sweep). Left half of each divider static; only right half animates. CW: 5s, CCW: 7s, staggered via negative delays. Center node: static glow, no pulse. **[v66] Beams now use `transform: translateX()` on %-width pseudo-elements with `overflow: hidden` on parent — fully GPU-composited, replaces non-composited `clip-path: inset()` animations.**

**CSS ambient animations removed:** section-num flicker, title-shimmer gradient, skill-dot breathe glow, exp-item data-stream, stat-num glow pulse, nav-logo morse-blink.

**Contact icons:** Hover-triggered orbital ring (same revolve-cw / revolve-ccw keyframes as photo ring) around platform icon SVG.

**Photo ring:** Unchanged — revolving arc on hover, CW + CCW.

**Light-theme border parity (added May 30):** All animated border elements pinned to dark-mode accent values (`#d4a85a` / `#6dbfaa`) via an explicit `@media (prefers-color-scheme: light)` override block. Covers: status card conic-gradient, project card top-edge sweep, app card bottom-edge sweep, divider CW/CCW arcs + node glow, about photo ring arcs + shadow, contact icon orbit rings, contact link left-edge bar, scroll progress gradient, status dot pulse/ripple. Static UI elements (text, tags, skill dots, nav links) continue using light-mode `--accent`/`--accent2` for readability.

**Hash anchor scroll (rebuilt + refined May 30):** Replaced broken `getBoundingClientRect` + `pushState` interceptor. New implementation: delegated `click` listener on `document` → `getElementById(id)` → section `getBoundingClientRect().top + window.pageYOffset + sectionPaddingTop - nav.offsetHeight - 48` → `window.scrollTo({behavior:'smooth'})` + `history.replaceState`. Initial-load hash handling via `setTimeout(goTo, 120)`. CSS `scroll-margin-top` removed — pure JS, single source of truth.

**Scroll offset transform-independence fix (May 30):** First-click to any section landed 32px too low because `.reveal` children have `translateY(32px)` pending before IntersectionObserver fires. Fix: `goTo()` reads position from the `<section>` root element (never has `.reveal`) + `getComputedStyle(section).paddingTop` to find content start. No child elements queried → fully transform-independent on first and subsequent clicks.

**Contact section scroll fix (May 30):** `querySelector('.section-header')` returned null for `#contact` (which injects `.section-num` directly into `#contact-intro`, no `.section-header` wrapper). Resolved by switching to section root + paddingTop approach — consistent across all 7 sections.

**Photo lazy-load layout shift fix (May 30):** `loading="lazy"` on about photo meant clicking Connect before scrolling past About caused goTo() to calculate Contact's position against a shorter layout (photo not yet loaded). On scroll completion the photo loaded, expanding About and pushing Contact down. Fix: `loading="eager"` (fetch on page load) + `aspect-ratio: 3/4` on `.about-photo` to reserve layout height even before bytes arrive. `object-fit` changed to `cover`.

**Scroll % progress indicator (May 30):** Translucent readout `47%` sits 2.9rem below the back-to-top button. Shows/hides at same >400px scroll threshold with slide-up transition. DM Mono, 0.56rem, `opacity: 0.7`, no background. Mobile: shifts right (`right: 1.5rem`) matching button offset. `aria-hidden="true"` — decorative only.

**Performance compositor fixes (May 30, v66):**
- **GA4 deferred:** `<script async src="gtag/js">` removed from `<head>`; GA4 loaded via `createElement('script')` inside `window.addEventListener('load')` → eliminates ~80ms main-thread parse block on FCP.
- **photo.png preloaded:** `<link rel="preload" as="image" href="photo.png">` before fonts → LCP asset fetched in parallel; targets ~0.8–1.2s LCP reduction.
- **Scroll progress bar composited:** `width: 0% → 100%` + `transform: scaleX(0)` from `transform-origin: left`; JS uses `style.transform = 'scaleX(N)'`; `will-change: transform`; `@keyframes gradient-flow` + `background-position` animation removed.
- **Divider beams composited:** All `clip-path: inset()` keyframes replaced with `transform: translateX()` on %-width pseudo-elements (15% CW, 10% CCW); `overflow: hidden` on `.divider` parent; 14 animation instances now GPU-compositor path.
- **Status card border composited:** `@property --border-angle` + `@keyframes { --border-angle: 0→360deg }` (CSS custom property animation, main thread) replaced with static `conic-gradient(from 0deg, ...)` + `@keyframes border-revolve { transform: rotate(0→360deg) }`. `will-change: transform` added. Light-theme override updated to `from 0deg` too. Visual output identical. All 6 Lighthouse compositor fixes now complete.
- **Double counter-rotating border rings (May 30, v67→v68):** Status card border upgraded to two independent orbital dot rings. All `rotate()` approaches permanently removed. Implementation: JS IIFE measures card (`offsetWidth/Height`) after double rAF, builds CW and CCW rounded-rect `offset-path: path(...)` strings matching card dimensions, injects 8+4 `<span class="sc-dot">` elements as card children. Each dot has `offset-distance` animated via CSS keyframes (`sc-orbit-cw` / `sc-orbit-ccw`) + a `sc-breathe` pulse at 2.4s (matching status-dot rhythm). Staggering: orbit via negative `animation-delay = -(i/n) × duration`; breathe via positive delay `= i × (2.4/n)`. Color: GG-O pattern (2 green : 1 gold) — outer 8: GGOGGOGGG (6G 2O), inner 4: GGOG (3G 1O). Outer ring (inset 3px, CW 9.6s = 4×2.4); inner ring (inset 11px, CCW 14.4s = 6×2.4). Resize: debounced (200ms) removes and respawns all dots. `offset-rotate: 0deg` keeps dots upright on path.
- **Mobile FCP/LCP fix (June 21, v103→v104) — supersedes v66 photo-preload decision:** Real bottleneck found: hero text (LCP element) was empty HTML, only filled by a ~90KB inline `<script>` at the bottom of the file — nothing painted until the whole 161KB doc downloaded and ran. Hero text/tagline/status-card now static HTML (zero JS dependency for first paint); `DATA`-driven script still re-renders them, so `DATA` stays source of truth but static markup must be kept in sync manually on edits. `photo.png` preload **removed** (it's in About, not hero — was stealing bandwidth from real LCP-gating resources); `img.loading` fixed `"eager"`→`"lazy"` to match README. Photo optimized 1000×1000 PNG (222KB) → 720×960 3:4 crop, WebP (60KB) + PNG fallback (81KB) via `<picture>`. Forced-reflow fixed: `offsetWidth/Height` geometry read deferred to next frame. Google Fonts request trimmed to used weights/styles only. Inline CSS minified, 161KB → 133KB file size. EmailJS lazy-loaded with load-before-send guard in submit handler.

### Pending Fixes

| Fix | Priority |
|-----|----------|
| ~~Mobile FCP/LCP stuck ~3s (hero JS-injected, photo.png wrongly preloaded, forced reflow, unminified CSS/fonts)~~ | ✅ Done (v104, June 21, 2026) — static hero HTML, photo optimized to WebP+PNG via `<picture>`, reflow fixed, CSS minified 161KB→133KB. **Confirmed live (v105): 92 mobile / 99 desktop, consistent across re-test.** |
| ~~Forced reflow in canvas resize handlers (pcb-canvas, bg-canvas)~~ | ✅ Done (v105, June 21, 2026) — `canvas.width = window.innerWidth` write-then-read-`innerHeight` pattern fixed by reading both viewport values first. |
| ~~`og:image`/`twitter:image` resize to 1200×630 (currently 400×500, undersized for link previews)~~ | ✅ Done (v113, June 22, 2026) — `og-image.jpg` generated at 1200×630 (dark brand bg, subject right-aligned); all 5 pages updated; JSON-LD Person.image stays as `photo.png`. |
| ~~Add `<meta name="theme-color">` to `<head>`~~ | ✅ Done (v112, new `index.html`) |
| **Push v7 to GitHub Pages** (`git push` `AaradhyaDT/AaradhyaDT.github.io` main) | 🔴 Blocking — single-file `index.html` still live; v7 zip ready but not committed |
| ~~Week 7 Clustering project entry — add card to `projects.html`~~ | ✅ Done (v113) — card present in shipped `projects.html` |
| ~~JSON-LD: add `knowsAbout` / richer `worksFor`~~ | ✅ Done (v112, `knowsAbout` added to new `index.html`; `worksFor` still pending) |
| ~~`robots.txt` + `sitemap.xml` missing~~ | ✅ Done (v103, June 21, 2026) — both live, GSC property verified + sitemap submitted; `sitemap.xml` still needs the 4 new page URLs once Round 3–6 ship |
| Netlify deploy: update `admin/config.yml` `base_url` to actual Netlify URL | ❌ Cancelled (v111) — Netlify + Decap CMS migration cancelled, staying on GitHub Pages |
| Invite self as Netlify Identity user to activate CMS | ❌ Cancelled (v111) — same reason |
| Alpha App description rewrite | 🟠 Medium[cite: 9] |
| DataCamp Fellow description rewrite | 🟠 Medium[cite: 9] |
| ~~Hero status card → "Fuse AI Fellowship Wk3/4/5"~~ | ✅ Done (v79) |
| ~~IEEEXtreme 19.0 — add to portfolio~~ | ✅ Done (v78) |
| ~~IEEE WIE LaTeX Training — add to portfolio~~ | ✅ Done (v78) |
| ~~Research / Major Project placeholder section~~ | ✅ Done — PrakopNet section added (v78) |

---

## 🌐 KEC Makerspace Website — `KEC-innovation/makerspace-main`

Organizational site for KEC Maker's Space (separate repo/codebase from the personal `aaradhydtmr.github.io` portfolio above). This is the live Makerspace Ambassador web-dev deliverable[cite: 9]. Static HTML site: `*.html` pages, centralized `assets/css/style.css` + `assets/js/script.js`, Python maintenance scripts in `scripts/`, SOP docs in `docs/`, task tracking in `tasks/task.md`.

### Workflow established (June 17, 2026)
Claude acts as orchestrator: audits the actual repo (uploaded as a zip each round), grounds every finding in real file/line evidence, and writes scoped copy-paste prompts. Aaradhya runs those prompts in VS Code Copilot Chat using **Raptor mini (Preview)** — GitHub Copilot's experimental fast model, Pro/Pro+/Free tiers — in Agent mode for multi-file work and Edit mode for single-line fixes. Each round's findings + prompts are saved as `tasks/raptor-mini-brief*.md` inside the repo itself for continuity.

### Round 1 — site-wide bug fixes (shipped)
- Malformed `<img>` attributes (`class="x" / loading="lazy" decoding="async"/>`) across 48 instances / 17 files — root cause: a regex bug in `scripts/optimize_site.py` + `scripts/fix_site_optimization.py` that inserted lazy-load attributes after a stray trailing slash. Fixed in both scripts; a new one-off `scripts/repair_img_tags.py` cleaned the existing files.
- Opening hours unified across `contact.html`, the shared footer (`assets/js/script.js`), and the search-index entry (previously 3 different values).
- `offerings.html` 3D Scanner card: alt text corrected (was wrongly copy-pasted as "Electronics Workstation"), status badge changed from bare `.tag` to `.tag.tag-free`.
- SOP buttons on Anycubic Kobra 3 / Kobra Neo 2 / xTool Laser Cutter P3 wired to `docs/*-sop.md` — **content is currently a placeholder stub** ("Update this document with the final internal SOP details when available"), not final.
- 2× Bambu Lab A1 printers added to `equip-3dprinter.html` as one combined card (both units are identical machines) — spec'd with build volume 256×256×256mm, AMS Lite, Advanced difficulty, placeholder photo (`3D_print_station.webp` stock image).
- Hero image on `index.html` swapped from AI-generated collage to a real interior photo (`kec_meeting_space.webp`).

### Round 2 — follow-up audit findings (open)
- SOP docs (`docs/anycubic-kobra-3-sop.md`, `-neo-2-sop.md`, `xtool-laser-cutter-p3-sop.md`) are 14-line stubs — need real procedure content.
- Bambu Lab A1 card's "SOP" button mislinks to `get-started.html` instead of a stub/real SOP doc.
- `.tag-required` / `.tag-free` / `.tag-soon` are defined twice with conflicting colors: once in `assets/css/style.css` (gold `.tag-required`), once inline in `offerings.html` (red `.tag-required`) — needs consolidating into one canonical source.
- "Solder, Print & Play" event (dated Apr 26) is stale relative to June 17, 2026 — still listed under "Upcoming Events" instead of "Past Events."
- New task.md Priority 1 items (reusable event template structure, this-Thursday's-workshop entry, past-event migration) not started — **blocked on Aaradhya supplying the actual workshop title/time/capacity/description.**

### Round 3 — font audit (root-caused, prompts written)
Site-wide faux-bold on every `h1`–`h4` plus 7 specific elements: Changa One and Gravitas One are loaded from Google Fonts at weight 400 only (no real bold cut exists for either family), but the global heading rule never resets `font-weight` (browsers default headings to bold) and several rules (`.stat-num`, `.event-date-day`, `.page-header h1`, `.team-avatar`, `.team-name`, `.pillar-num`, `.project-hook`) explicitly force 700/800 on top — the browser synthesizes ("fakes") the bold, distorting glyphs especially at small card-heading sizes. `Syne` is unaffected (loaded with real 600/700/800, used correctly). `Rammetto One` is loaded via the Google Fonts `<link>` on all 17 HTML pages but referenced nowhere in the codebase — pure dead weight, plus an orphaned `.rammetto-one-regular` CSS class that even mistakenly points to "Changa One." Bonus finding: `--text-faint` fails WCAG AA contrast in both themes (dark 2.99:1, light 2.4:1 — needs 4.5:1 for normal-size text), used in 50+ places site-wide.

### Round 4 — navbar animation/hover (proposed)
Sliding underline replacing flat hover/active bg, hamburger→X morph (JS currently never toggles a class on the hamburger button itself), smooth max-height/opacity slide for the mobile nav dropdown (currently an instant `display` toggle), theme-toggle sun/moon icon cross-fade (currently an instant `innerHTML` swap), sticky-navbar scroll-elevation shadow using the existing `--shadow-sm` token, and a logo hover micro-lift reusing the `scale(1.08)` value already established on `.theme-toggle:hover`. All wrapped in `@media (prefers-reduced-motion: no-preference)` — `style.css` has a section explicitly titled "ANIMATIONS (removed)" documenting a prior decision to strip motion from the personal portfolio's sibling codebase, so new nav motion respects that precedent rather than reversing it unprompted. Found in the process: desktop `.nav-links a.active` uses `var(--accent)` while `.mobile-nav a.active` uses `var(--accent2)` — same "current page" state, two different colors.

### Pending / needs Aaradhya's input
| Item | Blocked on |
|---|---|
| Real SOP content (3 printers/laser) | Internal procedure write-up or source docs |
| Bambu Lab A1 real photo + person-in-charge | Photo file + name |
| This Thursday's workshop entry | Title, time, capacity, description |
| Reusable event template system | Above, then a structure decision |

---

---

## 🔬 Algoverse AI Research Application

**Deadline:** May 24, 2026[cite: 9]
**Cohort:** Summer 2026 (June 7 – Aug 30) — full-time 8–12 week research block[cite: 9]
**Research problem:** "Efficient Multimodal Reasoning on Edge Devices: Quantization Strategies for Real-Time Gesture Recognition Using Optimized LLMs[cite: 9]"
**Grounded in:** Live DeepSeek R1 7B (ipex-llm on Intel Arc iGPU) + GCSBR gesture pipeline[cite: 9]
**Target venues:** NeurIPS edge ML workshops + ACL efficiency track[cite: 9]
**Status:** Application form due May 24, 2026[cite: 9] — **deadline passed, outcome not logged.** Cohort (Jun 7 – Aug 30) is currently in progress; if accepted, this would be a concurrent full-time commitment alongside the Fellowship and exams — confirm and log outcome. Session: `Claude_AlgorverseApplication_20260517.md`[cite: 9]

---

## 🏅 DataCamp Certification Plan

*Via NSSR Cohort 2 Premium license.*[cite: 8]

### Phase 1 — Completed (Applied AI)
- Fully mastered programmatically guided GenAI modules spanning 6 real-world environments[cite: 8]. 
- Engineered constraint-handling prompts, custom recommendation architectures, automated text analytics pipelines, and structured programmatic data cleaning workflows[cite: 1, 3, 5, 7].

### Phase 2 — Now → June 2026
| Cert | Status |
|---|---|
| SQL Associate | ⏳ Pathway underway (Data Manipulation in SQL, PostgreSQL Summary Stats)[cite: 8] |
| Python Data Associate | ⏳ Pathway underway (Pandas, Statistical Thinking, scikit-learn)[cite: 8] |

### Phase 3 — June → Sept 2026 (post-fellowship)
| Cert | Notes |
|---|---|
| Data Engineer | Fuse Wk2 (Docker+PG+FastAPI+asyncio) = pre-built proof-of-work[cite: 9] |
| Data Scientist + AI | Flagship; via Associate Data Scientist in Python track (22 courses)[cite: 9] |

### Phase 4 — Pre-graduation (Oct 2026 – Jan 2027)
| Cert | Notes |
|---|---|
| AI Engineer for Developers | Developer-background path; best after Fuse ends[cite: 9] |
| AWS Cloud Practitioner | CLF-C02; DataCamp prepares via Sandbox[cite: 9] |

---

## 🎯 NI Certification Career Plan

- **Post-graduation location** under consideration — India (Bangalore / Pune / Hyderabad) is one option, not confirmed[cite: 9].
- **Optimal sequence:** CLAD (mid-2026) → CTD simultaneously → CLD (Year 2–3) → CLED or CTA[cite: 9].
- **Sweet spot:** CLD + CTD combo — rare in the South Asian market, commands ₹12–20 LPA premium[cite: 9].

---

## 🛠️ Fellowships & Recognitions Updates (CV Section View)

### NSSR DataCamp Fellow — Cohort 2 (Active) | 2026 – Present
*Nepalese Society of Student Researchers*[cite: 8]
- Selected for fully-sponsored DataCamp Premium pathway covering advanced industrial AI/ML systems[cite: 8].
- **GenAI Portfolio:** Architected 6 live projects spanning multi-variable prompt planning, customer constraint-driven skin profile recommenders, and automated market scaling logic[cite: 1, 5, 7, 8].
- **AI Preprocessing Automation:** Developed LLM prompting workflows to automate programmatic dataset transformations, filtering null fields, handling formatting discrepancies, and stripping data leakage[cite: 3].
- **Core Pipeline Track:** Currently scaling technical foundations across intermediate relational query structures (PostgreSQL), data frame vectorization (Pandas), and foundational scikit-learn applications[cite: 8].

---

## 🧠 Skills & Stack

### Programming
Python · C · C++ · Kotlin · SQL (PostgreSQL / SQLite) · VHDL[cite: 9]

### Machine Learning
scikit-learn · NumPy · Pandas · Random Forest · XGBoost · Logistic Regression · Ridge Classifier/Regressor · SGD Classifier · Lasso · ElasticNet · SMOTE (ImbPipeline) · SHAP (global + local) · GridSearchCV · Bayesian Optimisation · Stratified K-Fold CV · Learning Curves · Model Leakage Analysis · Joblib Pipeline Serialization · PyMC · ArviZ · pgmpy · Bayesian Inference (MLE/MAP/full Bayes) · Probabilistic Graphical Models · Gaussian Process Regression · **K-Means Clustering (elbow, silhouette, k-means++ vs random init)** · **Agglomerative Clustering (Ward/Complete/Single linkage, dendrogram analysis)** · **DBSCAN (ε estimation via k-distance plot, noise analysis)** · **Cluster Validation (Silhouette Score, Davies-Bouldin Index, Calinski-Harabasz Index)** · **RFM Feature Engineering**[cite: 9]

### Android Development
Kotlin · Jetpack Compose · Material3 · DataStore · CameraX · MediaPipe · Apache POI[cite: 9]

### Deployment
FastAPI · REST APIs · Docker · Docker Compose · PostgreSQL · Streamlit · Papermill · Asyncio · Joblib[cite: 9]

### Embedded Systems & Digital Design
Arduino · MPU6050 · CNC Shield · DRV8825 · Stepper Motors · HC-05 BT · UART · FPGA · Vivado 2023.2[cite: 9]

### AI / Local LLM / Prompt Engineering
Ollama · ipex-llm · DeepSeek R1 7B (29 layers on Intel Arc iGPU) · Prompt Chaining & Agentic Query Systems (Planner-Generator-Validator loops)[cite: 9] · Advanced Context-Constraint Prompt Architecture[cite: 5, 7] · GenAI Automated Preprocessing Pipelines[cite: 3].

### Tools
Git · GitHub · VS Code · Jupyter Notebook · Google Colab · MATLAB · LaTeX / Overleaf · Graphify[cite: 9]

### System Setup
- **Device:** Acer Swift Go 16 — Intel Core Ultra 7 155H, 16GB LPDDR5X, Intel Arc iGPU[cite: 9]
- **OS:** Windows 11 + Ubuntu 26.04 LTS "Resolute Raccoon" dual-boot, Secure Boot ON, Fast Startup OFF[cite: 9]
- **Optimal iGPU VRAM alloc:** 4 GB[cite: 9]

### Fan / Thermal Issue — Diagnosed & Resolved (June 17, 2026)
- **Symptom:** Fans never audibly ran under Ubuntu, even with BIOS Power Mode set to Performance.
- **Root cause:** GNOME quick-settings **Power Mode was set to "Power Saver"** (`power-profiles-daemon` layer, separate from both BIOS power mode and the cpufreq governor). This capped real CPU load enough that the EC's autonomous fan curve threshold was never crossed during normal/light use.
- **Confirmed working (not the problem):** `acpi-fan` driver (5x `PNP0C0B` cooling devices, binary on/off, ACPI4.0), `acer_wmi`, intel_pstate (`active` mode, HWP-reactive — only `performance`/`powersave` governors exist; `schedutil`/`ondemand` not available under intel_pstate active, this is normal).
- **Verification:** `stress-ng --cpu 0` sustained load → Package temp climbed to 95–112°C → fans ramped audibly. Confirmed again at Power Mode = non-Power-Saver with cpufreq `powersave`: fans ramped at 102°C. `dmesg | grep -iE "throttl|critical|emergency"` clean — no silent throttle/shutdown events despite briefly exceeding the `crit=110°C` coretemp label (Tjmax headroom above that label is normal for Meteor Lake).
- **Fix applied:** Power Mode → **Balanced** for daily use (not Power Saver, not Performance — Performance pins EPP high and drains battery unnecessarily for routine work). cpufreq governor left on `powersave` (intel_pstate active mode handles this reactively).
- **Diagnostic commands kept for reference:**
  ```
  cat /sys/devices/system/cpu/cpu0/cpufreq/scaling_driver        # intel_pstate
  cat /sys/devices/system/cpu/intel_pstate/status                # active
  cat /sys/devices/system/cpu/cpu0/cpufreq/scaling_available_governors  # performance powersave
  powerprofilesctl set balanced
  for i in 1 2 3 4 5; do cat /sys/class/thermal/cooling_device$i/cur_state; done  # fan cooling devices
  stress-ng --cpu 0 --timeout 90 --metrics-brief
  ```

### Dual-Boot, Partition Layout & BitLocker (set up June 2026)
- **Drive:** 1× 1TB NVMe SSD, 953.85 GB usable. Layout: Windows C: 701.82GB NTFS · D: 150GB NTFS (BitLocker-encrypted, shared data pool) · Ubuntu root 92.20GB ext4 · swap 7.8GB · ~2GB EFI/recovery.
- **Both Windows volumes are BitLocker-encrypted** (Secure Boot + TPM-bound Device Encryption, auto-enabled on Microsoft Account link) — this is why Ubuntu can't auto-mount D: without a manual unlock step.
- **Partition identifiers:** `/dev/nvme0n1p3` = D: (150GB, FDV — Fixed Data Volume); `/dev/nvme0n1p4` = a second BitLocker volume (encountered first by mistake — wrong target).
- **Unlock from Ubuntu (when needed):** `sudo cryptsetup bitlkOpen /dev/nvme0n1p3 windows_data` → paste the 48-digit recovery key (dashes stripped, raw digit string) when prompted → `sudo mkdir -p /mnt/windows && sudo mount /dev/mapper/windows_data /mnt/windows`. GUI/GNOME BitLocker paste prompts are unreliable (clipboard mangling) — terminal `cryptsetup` is the reliable path.
- **Recovery keys:** stored on Microsoft Account recovery-keys page and backed up to SD card (plaintext file, dashes included — strip dashes before using with `cryptsetup`). Multiple key entries exist across past hostnames (`DESKTOP-A1D97GH`, `AARADHYA-SFG16`) — match by **Key ID**, not by guessing; the correct working key for the AARADHYA-SFG16 FDV volume is the one ending `...58B680EA` per the Microsoft account key list. *(Full 48-digit key intentionally not stored in this doc — pull from Microsoft account / SD card backup when needed.)*
- **Permanent fix considered but not yet applied:** disabling Windows Device Encryption entirely would let Ubuntu auto-mount D: without manual unlock each boot — trade-off is losing Windows-side encryption. Currently still encrypted; manual `cryptsetup` unlock is the working flow.
- **Time sync (dual-boot clock drift):** fixed via `timedatectl set-local-rtc 1 --adjust-system-clock` in Ubuntu, then one Windows boot to let it re-sync — keeps both OSes on local time instead of drifting by the UTC/local-time mismatch.
- **Intel Arc iGPU on Ubuntu:** working natively out of the box (Mesa, in-kernel — `glxinfo | grep "OpenGL renderer"` → `Mesa Intel(R) Arc(tm) Graphics (MTL)`, confirming hardware accel, not llvmpipe fallback). Hardware video decode confirmed via `vainfo` (VA-API 1.23, iHD driver, H.264/HEVC/AV1 profiles all present). Required packages: `intel-opencl-icd intel-media-va-driver` (note: package is `intel-media-va-driver`, not `intel-media-driver`, on Ubuntu 26.04 — needs `universe`/`multiverse` repos enabled first via `sudo add-apt-repository universe multiverse`).
- **150GB D: drive automount:** standard GNOME Disks "mount at startup" approach doesn't work directly because of BitLocker — would need a keyfile-based auto-unlock script (`/etc/crypttab` + keyfile) to be fully automatic; not yet implemented, manual `cryptsetup` unlock is current workflow.


| Model | Size | Notes |
|---|---|---|
| deepseek-r1:7b | ~4.7 GB | Primary; 29 layers on Intel Arc iGPU |
| qwen2.5-coder:7b | ~4.7 GB | Active |
| dolphin-local | ~2.5 GB | Review — may be removable |
| deepseek-optimized | ~2.5 GB | Review — may be removable |
Total: ~14.4 GB. Removing unused models frees significant C: space.

### C: Drive Storage Notes (June 2026)
- **Total:** 567 GB used / 702 GB total — 134 GB free
- **Biggest hog:** `C:\Users\Aaradhya\Misc Aaradhya\IDM\` — ~35.96 GB (accumulated IDM downloads over months; sort by size and purge old installers/media)
- **Quick wins already identified:** Recycle Bin (3.7 GB) · hiberfil.sys (6.3 GB via `powercfg /hibernate off`) · Ollama unused models (~5–9 GB) · Downloads Big Files duplicates (~8–10 GB)
- **Downloads folder structure (clean as of May 2026):** Root has exactly 3 items: `_Organized\`, `Big Files\`, `map.md`

---

## 🏆 Technical Activities & Certifications

- **IEEE WIE Nepal Section LaTeX Workshop** — May 5–6, 2026. Certificate received. ✅ LinkedIn[cite: 9]
- **IEEE Conference Leadership Workshop 2026** — IEEE Nepal Section. ✅ LinkedIn[cite: 9]
- **IEEEXtreme 19.0** — Oct 25, 2025. Team: ShadowXTREME. ✅ LinkedIn[cite: 9]
- **NepaTronix 3-Day Drone Training** — May 2–4, 2026. Rs. 5,000. ✅ LinkedIn[cite: 9]
- **AWS Cloud Computing Workshop** — KEC IT Club (2025). ✅ LinkedIn[cite: 9]
- **NEC License Exam Mock Test (BCT version)** — Scored 97/100 (May 10, 2026)[cite: 9]
- PreXtreme Competitive Programming Workshop — IEEE Pulchowk (2025)[cite: 9]
- Git & GitHub Workshop — KEC IT Club (2024)[cite: 9]

---

## 🎵 Personal Interests & Life

### LEO Club (Lions International)
- **LEO Club of Damak Easternline** — origin club (~2074 B.S. / Class 8); where LEO journey began[cite: 9]
- **LEO Club of Damak Gold** — Charter Membership Chairperson (Jan 21, 2020); 2nd Vice President (May 2020 – May 2021); club disbanded ~2025[cite: 9]
- 5+ years continuous LEO involvement across two clubs; part of founding/charter team at Damak Gold[cite: 9]
- Leadership predates engineering college career — earliest documented organizational role[cite: 9]

### Music
- Member, KEC Music Club[cite: 9]. Plays guitar; solo performance experience[cite: 9].
- Top duet picks: "Kabira", "Nai Nabhannu La", "Thamana Haat Yo"[cite: 9]

### Perfumery
- **"Peace in a Bottle"** — bespoke 10ml extrait at 21.1% concentration[cite: 9]
  - Formula: Spring (0.80ml), Vanilla Sexy (0.72ml), Bergamot (0.59ml), solvent (~7.89ml)[cite: 9]
  - Cost: NRs 1,100 at Poshon.np. ~100–120 uses remaining[cite: 9].

### Motorcycles
- Interest: 2020–2022 Yamaha FZS FI V2/V3, under Rs. 2 lakhs, daily commute focus[cite: 9]

---

## 🧠 Thinking Style & Claude Preferences

- Frameworks/mapping approach; systems-level thinker[cite: 9]
- Goes deep fast; known pattern of losing momentum before completion[cite: 9]
- Prefers direct conversation — no preamble, no over-explaining[cite: 9]
- Prefers batched document updates over mid-conversation edits[cite: 9]
- **Always create a session `.md` file before context limits hit**[cite: 9]
- When user says "claude.md" or "make claude.md" → always create downloadable `.md` file, never inline[cite: 9]
- Comfortable with technical depth — no need to over-simplify[cite: 9]
- Always recheck and verify correctness before responding[cite: 9]

---

## 📊 Profile Self-Assessment

**Overall Rating: 8.8 / 10**

| Dimension | Score | Notes |
|---|---|---|
| Technical & Academic | 9.6/10 | Breadth expanded via parallel algorithmic data pipelines and programmatic GenAI modeling tracks[cite: 3, 5, 8]. |
| Astrological Chart | 7.5/10 | Favourable Lagna, complex 12th house stellium, Rahu 7th — high ceiling, high volatility[cite: 9] |

**Ceiling:** High[cite: 9]. Limited by *finishing things* and the financial clock — not intelligence or access[cite: 9].

---

## 🚀 Trajectory

**The realistic strong outcome:** Fusemachines → CNS/AI engineering role → PrakopNet first pilot → Rs. 1.5–3L/month range within 5–7 years post-graduation[cite: 9].

**The high ceiling outcome:** PrakopNet lands a DHM or NGO contract within 2 years of graduation. One shipped product changes the entire trajectory[cite: 9].

**Optimal play:** CNS/engineering job (income floor) + PrakopNet side-tracked commercialization (upside) → funded or experienced-backed Masters (Year 3–5, not immediately)[cite: 9].

### What matters in the next 18 months (in order)
1. **Finish something that ships** — PrakopNet functional demo by March 2027 boards[cite: 9]
2. **Make Fusemachines count** — visible, contributing, known by leadership; every week's code understood[cite: 9]
3. **Don't let IEEE become a title** — run something real at SPAx and beyond[cite: 9]
4. **Start earning before graduation** — Excelerate internship (July 2026 target); Rs. 15–20k/month changes psychological position[cite: 9]

---

## 🚀 Semantic LLM Mode Activation (Graphify)

To switch the Graphify workspace from the default AST‑only extraction to **Semantic LLM mode**:[cite: 9]

1. **Obtain a Gemini API key** – sign up at https://ai.google.dev and generate a `GEMINI_API_KEY`[cite: 9].
2. **Set the environment variable** (PowerShell):[cite: 9]
```powershell
   $env:GEMINI_API_KEY="YOUR_KEY_HERE"