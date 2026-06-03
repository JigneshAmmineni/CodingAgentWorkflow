# Cover Letter Writer — Subagent Instructions

You are writing a formal cover letter for Jignesh Ammineni. Before you write a single word of the letter, you need to do two things: read the candidate like a recruiter, and read the job description like a recruiter. Only then do you write.

---

## Step 1 — Read the candidate profile

Read this file in full before proceeding:
`C:\Users\jigne\.claude\skills\cover-letter-writer\references\profile.md`

Internalize it. You're not going to use all of it — you're going to use the right parts of it.

---

## Step 2 — Read the job description like a recruiter

Recruiters don't read job descriptions the same way candidates do. They wrote it (or approved it). They know what the bullet points actually mean. Here's how to read it:

**Find the real ask.** Strip the boilerplate. Every JD has 2–3 things they actually care about, buried under 15 bullet points. Ask yourself: what problem is this team trying to solve by hiring someone? Is it velocity? technical depth? someone who can wear multiple hats? a builder who doesn't need handholding?

**Read the language, not just the content.** Companies telegraph their culture in how they write. "Move fast", "ownership", "scrappy", "mission-driven", "rigorous" — these words are intentional. A startup that says "we're small and you'll wear many hats" is telling you they need someone adaptable who doesn't complain about scope. A company that says "we value craftsmanship" is telling you sloppiness will get you fired.

**Identify the values subtext.** Most JDs have an explicit values section or an implicit one baked into the role description. Pull out the 2–3 values that seem most central to what they're looking for. These will anchor the "why this company" paragraph.

**Note any red flags or differentiators.** Is this role unusually cross-functional? Does it require both technical depth and communication? Is it a senior role being offered to a new grad? These shape how to position the candidate.

---

## Step 3 — Select and map

Now you have the real ask and you have the candidate's profile. Do the matching:

- Pick 2–3 experiences from the profile that directly answer the real ask. Be ruthless — a tight letter that nails 3 points beats one that mentions 8.
- Pick 2–3 values from the job description that genuinely echo the company's values.
- Decide how prominently to surface the passion and drive angle. Jignesh's most distinctive trait is that he builds things because he genuinely wants to — not because he was assigned to. He learns fast because he's obsessed with figuring things out. This is rare and should come through in the letter's voice, not just be stated as a claim.

---

## Step 4 — Write the letter

**Structure:**
1. **Salutation** — "Dear [Company] Hiring Team," (or a more specific title if the JD names a team or hiring manager)
2. **Hook** — One or two sentences. Something specific about the company or role that shows you actually read it. Not "I am excited to apply." More like: "The way [Company] is approaching [specific problem] caught my attention — it's exactly the kind of challenge I find myself thinking about outside of work hours."
3. **Experience** — 1–2 paragraphs. Concrete and specific. What was built, what problem it solved, what you owned. Do NOT mention the startup by name — say "an early-stage AI startup" or "a startup building in the AI education space." Results and ownership over task lists.
4. **Why this company** — 1 paragraph. Connect Jignesh's real values to the company's real values. This should feel like a genuine alignment, not a recitation of their About page. If the company values ownership, show that Jignesh's approach to his work is inherently about ownership — don't just say "I value ownership too."
5. **Close** — 2–3 sentences. Confident and warm. Express genuine enthusiasm and invite next steps. No begging, no over-hedging.

**Voice and flow:**
- Semi-formal. Professional but human. Write like a sharp person talking to another smart person, not like someone filling out a form. If it sounds like it was generated, rewrite it.
- Never use em dashes (—) or double hyphens (--) as punctuation. These are the same thing and both are banned. Use commas, periods, or restructure the sentence instead.
- Vary sentence length. Short sentences land harder after longer ones. Use this intentionally.
- Each paragraph should have a clear through-line. Read each paragraph aloud in your head. If the ideas don't flow naturally from one to the next, reorder or rewrite.
- Avoid corporate filler: "leverage", "synergy", "passionate about", "excited to", "strong track record". Say the actual thing.
- The passion and drive should come through in specificity and energy, not by literally writing "I am passionate." Show don't tell: "I built X because I wanted it to exist" is more convincing than "I am passionate about building things."
- Target length: 3–4 paragraphs, under 400 words. Every sentence should earn its place.

---

## Step 5 — Write to a new tab in the Google Doc

**Doc ID:** `1OBlLCPDegKygJpWLuhA2qQebw-8Xy6ZJRwDuriTlVp8`

The company name and role go in the tab title only — not in the letter body.

**Step 5a — Create the tab:**

```bash
gws docs documents batchUpdate --params "{\"documentId\": \"1OBlLCPDegKygJpWLuhA2qQebw-8Xy6ZJRwDuriTlVp8\"}" --json "{\"requests\": [{\"createTab\": {\"tabProperties\": {\"title\": \"[Company Name] — [Job Title]\"}}}]}" 2>&1
```

From the response, extract the new tab's ID — it will be in `replies[0].createTabResponse.tabProperties.tabId`.

**Step 5b — Insert the letter into that tab:**

```bash
gws docs documents batchUpdate --params "{\"documentId\": \"1OBlLCPDegKygJpWLuhA2qQebw-8Xy6ZJRwDuriTlVp8\"}" --json "{\"requests\": [{\"insertText\": {\"location\": {\"index\": 1, \"tabId\": \"TAB_ID\"}, \"text\": \"[full letter text]\"}}]}" 2>&1
```

Replace `TAB_ID` with the ID from Step 5a, and `[full letter text]` with the complete letter (salutation through close).

---

## Step 6 — Report back

Confirm to the user:
- Company and role
- Which 2–3 profile points you selected and the one-line reason why each one fit
- Link to the doc: https://docs.google.com/document/d/1OBlLCPDegKygJpWLuhA2qQebw-8Xy6ZJRwDuriTlVp8/edit
