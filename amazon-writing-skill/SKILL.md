---
name: amazon-writing-skill
description: Rewrite, draft, or review business and technical writing using Amazon-style objective communication and practical ASD-STE100 Simplified Technical English principles. Use for decision memos, status updates, requirements, plans, documentation, procedures, answers, and any text that needs to be concise, measurable, unambiguous, and accessible to non-experts.
---

# Amazon Writing

## Purpose

Write for a reader who must understand the message and decide what to do next. Combine:

- Amazon-style writing: lead with the answer, use evidence, remove subjective qualifiers, and apply the “so what?” test.
- Practical STE principles: use short, direct sentences, familiar words, one topic per sentence, active voice, consistent terms, and explicit instructions.

This skill is a practical writing aid. It does not certify compliance with ASD-STE100. For formal STE work, consult the current official standard and controlled dictionary.

## Workflow

1. Identify the reader, purpose, decision, action, and deadline.
2. Put the conclusion, request, or answer first.
3. Separate facts, assumptions, risks, decisions, and open questions.
4. Replace impressions with numbers, dates, comparisons, or named evidence. Never invent missing data.
5. Rewrite for simple, direct English.
6. Run the review checklist before delivering the text.

## Rules

### Be direct and concise

- Prefer sentences under 30 words. Split longer sentences when they contain more than one idea.
- Put one topic or action in each sentence. Use one action per procedural step.
- Use the active voice and name the actor: “The service writes the file,” not “The file is written.”
- Lead with the answer. For direct questions, answer with `yes`, `no`, a number, or `I don't know; I will follow up by [date].`
- Remove throat-clearing, repetition, inflated phrasing, and unnecessary background.

Prefer:

- “Because” over “due to the fact that.”
- “Could not” over “totally lacked the ability to.”
- “Use” over “make use of.”
- “Start” over “commence” or “initiate,” unless the domain requires a defined term.

### Be objective

- Replace adjectives and adverbs with observable facts.
- State the metric, unit, period, baseline, comparison, and cause when known.
- Replace “significantly,” “much faster,” “very successful,” and “better” with the measured result.
- Replace “nearly all,” “many,” “often,” and “soon” with a number, range, frequency, or date.
- Preserve uncertainty. State the confidence, assumption, or missing evidence instead of hiding it.
- Apply the “so what?” test: explain the consequence, decision, or action that follows from each important fact.

Example transformations:

| Avoid | Prefer |
| --- | --- |
| “Sales increased significantly in Q4.” | “Unit sales increased 40% in Q4 2011 versus Q4 2010.” |
| “We made the application much faster.” | “We reduced server-side p90 latency from 10 ms to 1 ms.” |
| “This will make the endeavor extremely successful.” | “This is expected to increase output by 2.5%.” |
| “The change would help the solution.” | “The change removes the timeout after 30 minutes.” |

If the data is unavailable, write “The data is not available” and identify the next step to obtain it.

### Use simple technical English

- Use common words and one term for one concept. Do not vary wording for style when consistency improves precision.
- Avoid idioms, metaphors, slang, buzzwords, noun piles, unnecessary nominalizations, and abstract wording.
- Prefer a concrete verb: “decide” instead of “make a decision”; “configure” instead of “perform configuration.”
- Keep technical terms when they are necessary, but explain them at first use.
- Expand an acronym on first use, then use the acronym consistently: “non-disclosure agreement (NDA).” Avoid an acronym when the short form is not needed.
- Resolve pronouns and references. Name the object instead of using “it,” “this,” “that,” or “they” when the reference could be unclear.
- Avoid ambiguous words such as “may,” “should,” “some,” “appropriate,” “quickly,” and “as needed” unless their meaning is defined.
- Use exact dates, times, units, and time zones when timing matters.

### Write procedures and requirements clearly

- State a condition before the action when the reader must know the condition first: “If the file exists, delete the file.”
- Use imperative steps: “Open the report.” “Enter the account number.”
- State one action and one expected result per step.
- Identify who performs each action when ownership is not obvious.
- State warnings, constraints, and failure conditions explicitly. Do not bury them in a long sentence.
- Use “must” for a requirement, “may” for permission, and “can” for capability. Do not use “should” when the action is mandatory.

## Review checklist

Before delivering the text, check:

- Does the first paragraph contain the answer, decision, request, or main result?
- Does every important claim have a number, date, comparison, source, or clearly stated uncertainty?
- Did I remove adjectives, adverbs, weasel words, buzzwords, and unsupported claims?
- Are sentences short enough and limited to one main idea?
- Is the actor clear, and is active voice used where it improves clarity?
- Are terms consistent, technical terms explained, and acronyms expanded once?
- Could a non-expert or non-native English reader interpret any sentence in two ways?
- Does each requirement or procedure state the condition, action, owner, and expected result?
- Does the text pass the “so what?” test for the intended decision or action?
- Did I preserve the original meaning, including limits and uncertainty?

## Output pattern

When rewriting, provide the revised text first. If useful, follow it with a short “Changes made” note that names only material changes, such as quantified claims, defined terms, removed ambiguity, or unresolved data gaps.

For an unanswered question, use this format:

> **Answer:** [Yes / No / number / I don't know]
> **Why:** [one fact-based sentence]
> **Next step:** [owner and date, only if follow-up is needed]

## Authority and limits

The Amazon principles in this skill are based on the user-provided “Write Like an Amazonian” notes. ASD-STE100 is maintained by the ASD Simplified Technical English Maintenance Group (STEMG). Use the official ASD-STE100 Issue 9 and its controlled dictionary for formal technical-documentation compliance:

- https://www.asd-ste100.org/
- https://www.asd-ste100.org/about_STE.html
- https://www.asd-ste100.org/STE_faq.html

Do not claim that a document is STE-compliant based only on this skill or on a readability score.
