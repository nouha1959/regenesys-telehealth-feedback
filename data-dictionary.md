# Regenesys Telehealth Feedback — Data Dictionary

Purpose: define every field the two Oct 30, 2026 Google Forms collect, so
anonymized aggregates exported later can be read consistently. This file
contains field definitions only — no responses, no names, no emails.

Reconciled against the live questionnaire on Oct 31, 2026 (read-only review;
no answers entered, nothing submitted). The live form presents 20 fields:
17 questions plus 3 follow-up fields (fields 5, 8, 20 below). Required fields
are field 1 and field 14 only. The 1–10 scales show no endpoint labels.

## Rules that apply to every export
- Raw responses stay in the private Google Sheets only ("Regenesys
  Telehealth Feedback — Responses" and "Regenesys Waitlist — Responses").
- Exports in this repo are anonymized aggregates only: counts, distributions,
  and rankings. Names, emails, and phone numbers are stripped before export.
- Free-text answers are paraphrased in any published summary, never
  attributed by name. Medical details are not collected; if a respondent
  writes one anyway, it is excluded from exports.
- The service is in pre-launch: no care is bookable yet, and no price or
  opening date is promised in any export or summary.

## Questionnaire fields (sections A–E, live numbering)
| Field | Type | Values / notes |
|---|---|---|
| used_telehealth_12mo | Yes/No | Field 1. Required on the form. |
| use_purpose | Multi-select | Weight management, Hormone health, Longevity & wellness, Primary care, Mental health, Other |
| use_frequency | Single choice | Once, A few times, Monthly, Ongoing subscription |
| top_frustration | Single choice (dropdown) | Rushed visits; Different clinician every time; Surprise charges or subscription traps; Support never answers; Impersonal, cookie-cutter plans; Other |
| what_happened_text | Open text | Field 5, follow-up to top_frustration. No medical details. |
| problem_severity_1_10 | Scale 1–10 | Field 6. Higher = bigger problem. No endpoint labels shown. |
| ever_quit | Yes/No | Field 7. |
| quit_reason_text | Open text | Field 8, follow-up to ever_quit. |
| current_monthly_spend | Band | $0, $1–50, $51–100, $101–200, $200+ |
| fair_monthly_price | Band | $0, up to $50, $51–100, $101–150, $150+ |
| switch_likelihood_1_10 | Scale 1–10 | Field 11. Likelihood of switching providers in the next 6 months. No endpoint labels shown. |
| feature_top3 | Pick top 3 | Same care team every time; Fast, human messaging; Plans built around my labs; Transparent flat pricing; A care coordinator who checks in; Community of people like me; Easy scheduling |
| dream_telehealth_text | Open text | Field 13. Co-creation answer; paraphrase only in summaries. |
| age_18_plus | Required checkbox | Field 14. The only required field besides field 1. |
| age_band | Single choice | 18–29, 30–44, 45–59, 60+ |
| state | Text | Field 16. Report only in aggregate (no small-cell breakdowns that could identify someone). |
| heard_about | Single choice | Instagram, TikTok, Friend, Search, Other |
| founding_community_optin | Yes/No | Field 18. |
| research_call_optin | Yes/No | Field 19. |
| call_email | Text, opt-in only | Field 20, follow-up to research_call_optin: "Email (only if you're open to a research call)". Lives only in the private call list, never in repo exports. |

## Waitlist fields
| Field | Type | Notes |
|---|---|---|
| first_name | Text | Required. Stripped from all exports. |
| email | Text | Required. Stripped from all exports. |
| phone | Text, optional | Text updates only. Stripped from all exports. |
| top_frustration | Text / choice as worded on the form | |
| dream_telehealth_text | Open text, optional | Added Oct 30, 2026. Paraphrase only in summaries. |

## Planned aggregate exports (not yet generated — forms were at 0 responses when verified Oct 30, 2026)
- Frustration rankings (field 4 counts)
- Problem severity distribution (field 6) and switch intent (field 11)
- Willingness-to-pay distribution (field 9 vs field 10)
- Feature top-3 counts (field 12)
- Dream-telehealth themes, paraphrased (field 13 and waitlist dream box)
