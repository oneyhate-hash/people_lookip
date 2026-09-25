#⭐ People Lookup JSON Generator — Professional GitHub Version
TABLE OF CONTENTS
Project Overview

Ethical Guidelines

JSON Template Structure

General Instructions

Multi‑Language Handling

JSON Syntax Rules

Field‑Specific Guidelines

Examples and Patterns

Validation Checklist

SECTION 1 — PROJECT OVERVIEW
This project defines a structured JSON output format for generating biographies from public, multi‑language sources.
It is designed for:

Pre‑interview validation

Contract screening

Public‑figure research

Multi‑source biography synthesis

Cross‑language comparison

The output must be valid JSON only, with no leading text, and must focus on lasting contributions in science, technology, society, and culture.

SECTION 2 — ETHICAL GUIDELINES
Use only publicly available sources (Wikipedia, public archives, news, public databases).

Do not include private, speculative, or harmful information.

Skip any field with no public data.

Avoid political controversies and non‑public personal details.

Sensitive fields (relationships, children, criminal issues) must only be filled for public figures with documented sources.

SECTION 3 — JSON TEMPLATE STRUCTURE
Produce JSON with the following structure (skip unknown fields):

Code
{
  "name": "<name>",
  "language_info": "<list of languages received, their content and interest>",
  "years": "<birth/death details with ages>",
  "origin": "<ancestral details>",
  "race/religion of ancestors": "<details for parents and grandparents>",
  "age now": <N>,
  "locations": ["location details with age ranges"],
  "relationships": [{"specific details on family, marriages with ages"}],
  "number_of_children": <N or "known 0">,
  "number_of_known_offspring_total": <M>,
  "children_details": [{"age, survival, descendants, sex, mother if needed"}],
  "offspring_total": "<summary of all known offspring>",
  "spouse_details": ["relevant details for each spouse"],
  "education": [{"school, years with ages, location, degree"}],
  "companies": [{"name, years with ages, role, location, employees"}],
  "criminal_or_drug_issues": "<major issues with times and penalties>",
  "intellectual output": ["major items with years, effects, meaning"],
  "artistic output": ["major items with years, effects, meaning"],
  "other_careers": ["careers with length"],
  "public_achievements_and_honors": ["awards, recognitions with years and ages"],
  "notable_contributions_to_society_culture": "<summary of impacts with years and effects>",
  "philanthropy_and_social_involvement": ["charitable work, foundations with years and scope"],
  "travel_and_global_exposure": ["key travels for professional/cultural reasons with locations, years, ages"],
  "mentorship_and_influences": ["mentors, mentees, influences with public details"],
  "legacy_and_posthumous_impact": "<ongoing effects, memorials with public context>",
  "language_comments": ["variations by language"],
  "language_sentiment": ["analysis for each language: positive/negative, fair/unfair, significant"],
  "comments": "<general commentary>",
  "life_timeline": "<ASCII timeline under 200 chars width>"
}
SECTION 4 — GENERAL INSTRUCTIONS
Skip any field with no public data.

Always include ages when listing years.

Avoid generalizations; be specific.

Focus on lasting contributions.

Mark AI‑inferred info with underscores.

Avoid repeating information across fields.

Sensitive fields only for public figures.

SECTION 5 — MULTI‑LANGUAGE HANDLING
Input may come from multiple languages.

Output must be in English.

Label contradictions clearly (e.g., "english_wikipedia": "value" vs "spanish_wikipedia": "value").

Include minority viewpoints when significant.

If sources agree, no need to highlight differences.

SECTION 6 — JSON SYNTAX RULES
All strings must be quoted.

Arrays use [], objects use {}.

No trailing commas.

Numbers may be unquoted only when standalone.

Output must be valid JSON (test with jsonlint.com if needed).

SECTION 7 — FIELD‑SPECIFIC GUIDELINES
Relationships: list names, ages, and public details.

Offspring: only for public figures.

Intellectual/Artistic Output: include effects and meaning.

New Fields: Achievements, Contributions, Philanthropy, Travel, Mentorship, Legacy.

SECTION 8 — EXAMPLES AND PATTERNS
Good Example:

Code
"number_of_children": {
  "english_wikipedia": 3,
  "spanish_wikipedia": 7
}
Bad Example:

Code
"Napoleon's age": 9-15
Correct form:

Code
"Napoleon's age": "9-15"
Skip empty arrays/objects; do not include null or unknown.

SECTION 9 — VALIDATION CHECKLIST
No empty arrays or objects.

All years include ages.

Sentiment analysis must be balanced and factual.

Timeline must be ASCII‑only and under 200 characters wide.

Output must be pure JSON with no leading text.

No private or speculative data. people_lookip
