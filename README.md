# MTLE Retake Mock Exam Hub

A static, Vercel-ready website containing 10 independent subject practice banks (100 questions each; 1,000 total).

## Included mock exams

1. Clinical Chemistry
2. Hematology
3. Clinical Microscopy
4. Clinical Microbiology
5. Parasitology
6. Blood Banking / Immunohematology
7. Immunology & Serology
8. Histopathology
9. Molecular Biology
10. MT Laws & Ethics

Every bank contains **60 MCQs, 20 two-statement questions, and 20 Morse/combination questions**. Every item has an answer and rationale. Practice mode reveals explanations after each answer. Exam mode hides explanations until submission and uses a 120-minute practice timer. The timer is a study setting, not a representation of official examination timing.

## Source alignment and limitations

The project uses the uploaded updated MTLE Table of Specifications (TOS), Clinical Chemistry, Hematology, Clinical Microscopy Day 1/Day 2, and Histopathology transes, plus the updated GOD BLESS recall compilation.

The TOS officially combines several content areas: Microbiology + Parasitology; Blood Banking + Immunology/Serology; and Histopathology + MT Laws/Ethics. The separate 100-item banks are a focused practice design and **do not imply that each is an independent 100-item official board subject**. Molecular biology topics appear within the official TOS of other subjects and are separated here for focused practice only.

No separate dedicated lecture transes for Microbiology/Parasitology, Blood Banking/Immunohematology, Immunology/Serology, Molecular Biology, or MT Laws/Ethics were present in the lecture set used for this build. Those banks are therefore based on the TOS and the relevant recall themes, with foundational context clearly distinguished from dedicated lecture coverage. Laws/Ethics items should be checked against the latest official texts, implementing rules and PRC issuances before relying on them for current legal requirements. The TOS prints “RA968”; the site uses RA 10968 for the Philippine Qualifications Framework Act.

Recall items are not copied wholesale as a verified answer key. These are newly phrased practice questions. Do not treat the recall compilation's proposed answers as automatically validated.

## Deploy to Vercel

### Option 1: GitHub import
1. Extract this ZIP.
2. Create a new GitHub repository and upload the contents of this folder to the repository root.
3. In Vercel, choose **Add New → Project**, import the repository, and keep the Framework Preset as **Other**.
4. Leave Build Command and Output Directory empty/default; this is a static site.
5. Deploy.

### Option 2: Vercel CLI

Install/use the Vercel CLI, open a terminal in this folder, and run:

```bash
npx vercel
```

Follow the prompts. For production deployment, run `npx vercel --prod`.

## Files

- `index.html` — responsive mock exam app
- `questions.js` — all 1,000 question records, answer keys and rationales
- `vercel.json` — static routing configuration

No database or environment variables are required. Attempt progress is saved in the browser's local storage on the same device/browser.
