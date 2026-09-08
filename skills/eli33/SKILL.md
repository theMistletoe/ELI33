---
name: eli33
description: "Explain complex topics accurately and respectfully for an intelligent adult non-specialist, defaulting to a 33-year-old audience. Use when the user says 'ELI33', '33歳向けに説明して', '成人にも分かるように', '専門外の社会人向けに', 'explain like I am 33', 'explain like I am', 'ELI5', 'explain this to my', 'break this down for', 'simplify this for', or requests an explanation for a named age, education level, profession, relationship, or non-technical audience. Preserve the explicitly requested audience; use the age-33 default only when none is given."
---

# Explain Like I Am 33 (ELI33)

Explain complex topics so the intended audience can understand them without sacrificing correctness or treating them condescendingly.

## Step 1: Identify the Audience

First identify any audience explicitly stated by the user. Adapt to its age, education, profession, relationship, vocabulary, interests, and goals. **Only when no audience is stated, default to Age 33.** `ELI5` remains a supported trigger, but by itself uses the Age 33 default; an explicit request such as “like a 5-year-old” overrides it.

### Ages
| Audience | Style |
|----------|-------|
| Age 5 | Very simple words, concrete examples, and short sentences. Use playful analogies without talking down. |
| Age 10 | Elementary-school vocabulary and basic cause-and-effect; school, sports, or game examples can help. |
| Age 15 | Some abstraction and defined terminology; conversational but not forced slang. |
| Age 20-39 | Clear, direct adult explanation using daily life, work, and money where relevant. |
| **Age 33 (default)** | Assume general adult knowledge plus work and life experience, but no specialist knowledge of the subject. |
| Age 40+ | Respectful adult tone; use relevant career, household, family, or financial contexts without stereotypes. |

### Grade / Education Levels
| Audience | Style |
|----------|-------|
| 5th grade | Simple vocabulary, concrete examples, and immediately defined essential terms. |
| Middle school | Basic terminology with definitions and step-by-step logic. |
| Senior High | Moderate complexity; introduce and explain proper terms. |
| College Student | Academic framing, technical terms with context, and theory plus application. |
| Graduate school | Assume strong foundations; emphasize nuance, trade-offs, edge cases, and precision. |

### Job Roles
| Audience | Focus |
|----------|-------|
| Manager | Impact, timeline, risk, cost, decisions, and team implications |
| Engineer | Mechanism, architecture, implementation, performance, and maintainability |
| Designer | User experience, interaction, visual impact, and accessibility |
| Director | Strategy, ROI, competitive position, and resource allocation |
| Colleague | Shared work, practical context, and collaboration needs |
| Product Manager | User value, priorities, scope, and build-versus-skip decisions |

### Relationships
| Audience | Tone and framing |
|----------|------------------|
| Partner | Warm and conversational; shared routines where relevant |
| Parents | Respectful and clear; familiar examples without assumptions about technical ability |
| Children | Encouraging, concrete, and age-appropriate |
| Friend | Casual and direct; shared interests when known |

## Step 2: Understand the Subject

Before explaining, establish the essential what, why, and causal mechanism. Read relevant source material and determine the root cause of errors rather than paraphrasing their surface text. Preserve important qualifications and uncertainty.

## Step 3: Craft the Explanation

### Default Age-33 Rules

- Lead with the conclusion or key point.
- Do not avoid necessary technical terms; define each at first use in plain language.
- Use concrete examples from adult life when helpful: work, household finances, contracts, health management, or digital services.
- Explain the mechanism, benefits, drawbacks, and practical decision criteria.
- Avoid childish phrasing, fake enthusiasm, and any implication that simplicity means low intelligence.
- Maintain accuracy. Simplify presentation and supply missing prerequisites rather than distorting the subject.

### Structure

For the default audience, normally use this order:

1. **Key point** — state the conclusion in one or two sentences.
2. **How it works** — explain the causal mechanism and define necessary terms.
3. **Concrete example** — connect the mechanism to adult daily life or work.
4. **Caveat or trade-off** — explain costs, limits, risks, or alternatives.
5. **What it means in practice** — give useful judgment criteria or next steps.

Change the structure when the user’s explicit audience or task calls for it. Use analogies only when they improve understanding. Do not default to toys, animals, candy, or other preschool imagery for adults.

### Language Calibration

For the default 33-year-old non-specialist:
- Write clearly and peer-to-peer with moderate information density.
- Use precise terminology when it matters, defining it on first appearance.
- Assume ordinary adult knowledge, not domain expertise.
- Add the prerequisites needed for accuracy; do not over-simplify away causes, uncertainty, or trade-offs.

For children or other explicitly simple audiences, use age-appropriate vocabulary and shorter steps while retaining the core truth. For specialists, use established terminology and focus on architecture, evidence, edge cases, and trade-offs. For business audiences, lead with outcomes and decisions and include implementation detail only when relevant.

### Tone Matching

- **Default Age 33:** direct, calm, respectful, and collaborative—an informed colleague bringing another adult up to speed.
- **Children:** warm and encouraging, never patronizing.
- **Teenagers:** conversational without forced slang.
- **Professionals:** confident and concise; respect existing expertise while filling domain gaps.
- **Family or friends:** natural and patient without stereotyping.

## Examples

**User:** “ELI33: What is a database index?”
**Audience:** Age 33 (default)
**Response style:** “A database index is an extra, searchable data structure that lets the database find records without scanning every row. It works like the index in a reference book—or a searchable register of invoices at work—that points to the full record. This makes reads much faster, but every insert or update must also maintain the index, consuming storage and adding write cost. In practice, index fields you search or sort often, not every field.”

**User:** “Explain API rate limiting to my manager.”
**Audience:** Manager
**Response style:** Lead with customer and business impact, define the request limit, outline why failures occur at peak traffic, compare reducing calls with buying capacity, and end with a decision recommendation.

**User:** “Break down merge conflicts for a 5th grader.”
**Audience:** 5th grade (explicit override)
**Response style:** Use a shared school-document example, define the conflict as two incompatible edits to the same part, and walk through choosing or combining the changes.

## Final Check

Before answering, verify that the explanation matches any explicit audience; otherwise verify it fits Age 33. Confirm that it leads with the point, defines necessary terms, includes a relevant example when useful, retains accuracy and trade-offs, and avoids condescension.
