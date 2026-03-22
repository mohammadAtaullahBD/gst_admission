# Deep Research Prompt: EEE Program Analysis — GST Cluster Universities (Bangladesh)

## Mission

You are a research agent conducting a rigorous, source-grounded comparative analysis of Electrical and Electronic Engineering (EEE) programs across 10 public universities in the GST admission cluster in Bangladesh. The output must be detailed enough to help a prospective BSc EEE student choose the best university for a career path in robotics and a long-term goal of pursuing a fully-funded MS abroad (DAAD/Germany or MEXT/Japan).

Do not hallucinate data. If a specific figure (e.g., publication count, lab count) is not found, explicitly state "Not publicly available" and provide a reasoned estimate labeled as such.

---

## Universities Under Investigation

| # | University | Short Name | EEE Seats | EECE Seats | Website |
|---|---|---|---|---|---|
| 1 | Jashore University of Science and Technology, Jashore | JUST | 35 | — | just.edu.bd |
| 2 | Noakhali Science and Technology University, Noakhali | NSTU | 48 | — | nstu.edu.bd |
| 3 | Pabna University of Science and Technology, Pabna | PUST | 40 | 40 | pust.ac.bd |
| 4 | Islamic University, Kushtia | IU | 50 | — | iu.ac.bd |
| 5 | Patuakhali Science and Technology University, Patuakhali | PSTU | Unknown | - | pstu.ac.bd |
| 6 | Jatiya Kabi Kazi Nazrul Islam University, Mymensingh | JKKNIU | 40 | — | jkkniu.edu.bd |
| 7 | Begum Rokeya University, Rangpur | BRUR | 55 | — | brur.ac.bd |
| 8 | Jamalpur Science and Technology University | JSTU | 30 | — | jstu.ac.bd |
| 9 | Gopalganj Science and Technology University | GSTU | 40 | — | gstu.edu.bd |
| 10 | Netrokona University | NEU | 40 | — | neu.ac.bd |

> Note: If any university does not offer EEE or EECE at all (e.g., PSTU seat count unconfirmed), verify first and exclude it from ranking if confirmed absent.

---

## Research Strategy (Per University)

For each university, execute the following steps in order. Do not skip steps.

### Step 1 — Establish baseline
- Search: `"[University Name]" EEE department faculty`
- Fetch the university's official EEE/EECE department page at `https://[domain]/eee` or equivalent.
- Confirm whether EEE/EECE program exists and is currently active.

### Step 2 — Faculty intelligence
- Search: `"[University Name]" EEE faculty PhD research publication`
- Look for:
  - Full faculty list with designations (Professor / Associate Professor / Assistant Professor / Lecturer)
  - PhD completion country and institution (e.g., Japan, Germany, Australia, UK, USA, South Korea, India, Bangladesh)
  - Google Scholar or ResearchGate profiles if linked
  - Research interests per faculty member

### Step 3 — Research output
- Search: `"[University Name]" EEE Scopus IEEE publication 2020 2021 2022 2023 2024`
- Search: `site:scholar.google.com "[University Name]" electrical engineering`
- Look for:
  - Scopus or Web of Science indexed journal papers
  - IEEE conference and journal publications
  - UGC-funded research grants
  - International research collaborations

### Step 4 — Rankings and recognition
- Search: `"[University Name]" QS ranking THE ranking Scimago webometrics 2024 2025 2026`
- Check `webometrics.info` for the university's Bangladesh and world rank.

### Step 5 — Labs and infrastructure
- Search: `"[University Name]" EEE laboratory equipment microcontroller power electronics MATLAB`
- Fetch the labs or facilities page if available.
- Note named labs, equipment types, and condition.

### Step 6 — IEEE Student Branch and clubs
- Search: `"[University Name]" IEEE student branch robotics club technical competition`
- Check `ewh.ieee.org` or `ieeebd.org` for registered student branches in Bangladesh.

### Step 7 — Academic stability
- Search: `"[University Name]" session jam academic calendar disruption 2023 2024`
- Note any known political or administrative disruptions to the academic calendar.

---

## Data Points to Collect Per University

Use the exact field names below. Fill every field; write "Unknown" only when genuinely not findable after searching.

```
UNIVERSITY: [Full Name] ([Short Name])
DOMAIN: [website URL]
EEE_SEATS: [number from table above]
EECE_SEATS: [number or "None"]
EEE_ESTABLISHED: [Year, or "same as university founding", or "Unknown"]
UNIVERSITY_STATUS: [Mature | Developing | Newly Established]
EEE_STATUS: [Mature | Developing | Newly Established]

FACULTY_TOTAL: [number or "Unknown"]
FACULTY_PROFESSOR: [number or "Unknown"]
FACULTY_ASSOC_PROF: [number or "Unknown"]
FACULTY_ASST_PROF: [number or "Unknown"]
FACULTY_LECTURER: [number or "Unknown"]
PHD_PERCENTAGE: [e.g., "60%" or "4 out of 7" or "Unknown"]
PHD_COUNTRIES: [e.g., "Japan (2), Australia (1), Bangladesh (1)" or "Unknown"]
RESEARCH_INTERESTS: [comma-separated list, e.g., "Power Systems, Renewable Energy, VLSI, ML, Robotics, Embedded Systems"]

PUBLICATIONS_LAST_5YR: [confirmed number, OR "Estimated: Low/Medium/High — [1-line reasoning]"]
SCOPUS_INDEXED: [Yes | Partial | Unknown]
RESEARCH_CENTERS: [named labs/centers, or "None identified"]
UGC_GRANTS: [Yes | No | Unknown]
INTL_COLLABORATIONS: [list if found, or "None identified"]
MS_PHD_PROGRAMS: [Yes | No | Under development]

LABS_AVAILABLE: [named labs, e.g., "Electronics Lab, Power Systems Lab, Microcontroller Lab"]
LAB_CONDITION: [Modern | Adequate | Basic | Unknown]
IEEE_LIBRARY_ACCESS: [Yes | No | Unknown]
SIMULATION_SOFTWARE: [e.g., "MATLAB, Proteus, LTSpice" or "Unknown"]

IEEE_STUDENT_BRANCH: [Yes | No | Unknown]
ROBOTICS_CLUB: [Yes | No | Unknown]
INDUSTRY_CONNECTIONS: [list if found, or "None identified"]
PLACEMENT_RATE: [percentage or "Unknown"]

QS_RANK_ASIA: [rank or "Not ranked"]
THE_RANK_WORLD: [rank or "Not ranked"]
WEBOMETRICS_BD_RANK: [rank or "Unknown"]
SCIMAGO_RANK: [rank or "Unknown"]

SESSION_JAM_RISK: [Low | Medium | High | Unknown]
STUDENT_FACULTY_RATIO: [e.g., "25:1" or "Unknown"]

KNOWN_ISSUES: [bullet list — e.g., faculty shortage, remote location, new dept, political disruptions]
NOTABLE_STRENGTHS: [bullet list — standout positives]

DATA_CONFIDENCE: [High | Medium | Low] (your overall confidence in the data collected for this university)
SOURCES_USED: [list URLs or source names used]
```

---

## Scoring & Ranking Criteria

After completing all profiles, score each university on the following criteria (0–10 per criterion). Apply the weighting formula to get a final weighted score.

| Criterion | Weight | Scoring Guidance |
|---|---|---|
| Research strength | 25% | PhD %, publication count, Scopus indexing, research centers, international collaborations |
| Lab facilities & infrastructure | 20% | Named labs, modern equipment, simulation software, IEEE digital library access |
| International ranking | 20% | QS Asia, THE World, Scimago, Webometrics BD rank — higher = higher score; unranked = 2–3/10 |
| Scholarship preparation potential | 20% | Research culture, faculty mentorship, MS/PhD program availability, IEEE student branch, proven DAAD/MEXT track record |
| Academic stability & campus environment | 15% | Session jam history, student-faculty ratio, technical clubs, extracurriculars |

**Weighted Score formula:**
```
Score = (Research × 0.25) + (Labs × 0.20) + (Ranking × 0.20) + (Scholarship × 0.20) + (Stability × 0.15)
```

**Tiers:**
- Tier 1: Weighted Score ≥ 7.5
- Tier 2: Weighted Score 5.5–7.4
- Tier 3: Weighted Score < 5.5

**Important scoring rules:**
- Unknown data defaults to a conservative score of 3/10 for that criterion — do not assume neutral.
- A newly established department with no track record cannot score above 4/10 for Research or Scholarship, regardless of parent university reputation.
- Do not award bonus points for potential; score based on current, evidenced reality.

---

## Required Output Format

Deliver your output in the following structure — in this exact order.

---

### Output 1 — University Profiles (JSON file)

Produce a single downloadable JSON file named `gst_eee_university_profiles.json`.

The JSON must follow this schema exactly:

```json
{
  "metadata": {
    "generated_by": "AI Research Agent",
    "purpose": "GST EEE University Comparison — Bangladesh",
    "student_context": "BSc EEE → MS abroad (DAAD/MEXT) → Robotics career",
    "date": "[today's date]"
  },
  "universities": [
    {
      "short_name": "JUST",
      "full_name": "Jashore University of Science and Technology",
      "domain": "just.edu.bd",
      "eee_seats": 35,
      "eece_seats": null,
      "eee_established": "...",
      "university_status": "...",
      "eee_status": "...",
      "faculty": {
        "total": null,
        "professor": null,
        "assoc_prof": null,
        "asst_prof": null,
        "lecturer": null,
        "phd_percentage": "...",
        "phd_countries": "...",
        "research_interests": []
      },
      "research": {
        "publications_last_5yr": "...",
        "scopus_indexed": "...",
        "research_centers": [],
        "ugc_grants": "...",
        "intl_collaborations": [],
        "ms_phd_programs": "..."
      },
      "infrastructure": {
        "labs_available": [],
        "lab_condition": "...",
        "ieee_library_access": "...",
        "simulation_software": []
      },
      "environment": {
        "ieee_student_branch": "...",
        "robotics_club": "...",
        "industry_connections": [],
        "placement_rate": "...",
        "session_jam_risk": "...",
        "student_faculty_ratio": "..."
      },
      "rankings": {
        "qs_rank_asia": "...",
        "the_rank_world": "...",
        "webometrics_bd_rank": "...",
        "scimago_rank": "..."
      },
      "assessment": {
        "known_issues": [],
        "notable_strengths": [],
        "data_confidence": "...",
        "sources_used": []
      },
      "scores": {
        "research": null,
        "labs": null,
        "ranking": null,
        "scholarship_prep": null,
        "stability": null,
        "weighted_total": null,
        "tier": null
      }
    }
  ]
}
```

Repeat the university object for all 10 universities. Scores must be filled in with numerical values (floats to 1 decimal place). `weighted_total` must be computed using the formula above.

---

### Output 2 — Interactive HTML Dashboard

Build a self-contained single-file HTML page (no external dependencies except CDN-hosted Chart.js and a Google Font) that:

1. **Embeds the full JSON data** inline in a `<script>` tag (do not fetch from an external file)
2. **Ranked comparison table** with columns:
   `Rank | University | Research (25%) | Labs (20%) | Intl Ranking (20%) | Scholarship Prep (20%) | Stability (15%) | Weighted Score | Tier`
   - Rows sorted by weighted score descending
   - Tier badge colored: Tier 1 = green, Tier 2 = amber, Tier 3 = red
   - Score cells color-coded: ≥7 green, 5–6.9 amber, <5 red
3. **Strengths & Weaknesses summary table** with columns:
   `University | Top 2 Strengths | Top 2 Weaknesses | Best For`
4. **Bar chart** (Chart.js) showing weighted scores for all universities, sorted highest to lowest
5. **University detail cards** — clicking any row in the table expands a detail panel showing all collected data fields for that university
6. **Final Recommendation section** at the bottom answering the student's question (see Section 4 below)

Name the file: `gst_eee_dashboard.html`

---

### Output 3 — Strengths & Weaknesses Table

Included inside the HTML dashboard, but also printed as plain text in your response for quick reference.

Columns: `University | Top 2 Strengths | Top 2 Weaknesses | Best For`

---

### Output 4 — Final Recommendation

Answer this specific question inside the HTML dashboard and in your plain response:

> *"Which university from this list offers the best EEE program for a student whose goal is robotics research, a CGPA of 3.5+, and a fully funded MS abroad (DAAD/Germany or MEXT/Japan)?"*

Provide:
- **First choice** — with justification covering: faculty PhD quality, research environment, ranking, and how it directly helps the student's DAAD/MEXT application
- **Second choice** — backup with clear reasoning
- **Dark horse pick** — a less obvious university that may be underrated given the student's specific goals
- **BSc action plan** — for each recommended university, list 4–5 specific things the student should do during their BSc years to maximize their chances of a full scholarship abroad

---

## Quality Standards

- Cite sources inline (URL or source name) for every non-trivial factual claim.
- Clearly distinguish confirmed data from reasoned estimates using labels: `[Confirmed]` vs `[Estimated]`.
- If a university does not offer EEE or EECE, state this explicitly and exclude it from scoring.
- Do not inflate scores for universities with insufficient data. Missing data = conservative score.
- Prefer: official university websites → UGC Bangladesh annual reports → IEEE Bangladesh Section → Scopus/Scimago → Google Scholar → reputable Bangladeshi news sources.
- Where sources conflict, note the conflict and use the more recent or authoritative one.
- `DATA_CONFIDENCE` must honestly reflect how much of the data is confirmed vs estimated.

---

## Student Context (Critical — Do Not Ignore)

The student this research serves:
- Completed HSC 2025, Dhaka Board — currently in the university admission phase in Bangladesh
- Target degree: BSc in EEE (prefers EEE for robotics; also open to EECE)
- Long-term goal: fully funded MS abroad (DAAD/Germany = first priority, MEXT/Japan = second)
- Career goal: robotics engineer working in Germany, Japan, or equivalent high-income country
- Already sat for and was not selected at (or did not get): BUET, CUET, KUET, RUET, CU, KU, DU, JnU, JU, RU, SUST, HSTU
- The GST cluster (these 10 universities) is one of two remaining options; the other is DU Technology Unit (6 colleges)

**Weighting instruction:** A smaller or lower-ranked university with genuinely active research faculty, a strong IEEE student branch, and a culture of graduate-level research may outrank a larger university with passive faculty and weak research output — because the former better serves this student's DAAD/MEXT pathway.
