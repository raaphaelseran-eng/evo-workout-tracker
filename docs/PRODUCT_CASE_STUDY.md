# evo — Product case study

## Opportunity

Workout data are often written in a hurry: abbreviated exercise names, quick sets, values placed before or after a movement and comments mixed into a note. A structured form can interrupt the flow; a plain note cannot be analyzed automatically. The objective was to combine the low friction of a note with the value of a structured training journal.

## Workflow

1. **Write:** capture a session using informal text.
2. **Understand:** identify exercises and sets in the note, and flag name ambiguity when needed.
3. **Review:** allow the user to inspect, edit and correct the interpreted session.
4. **Organize:** maintain session and exercise history.
5. **Learn:** show progress charts, training activity and personal-record indicators.

## Features demonstrated in the screenshots

- Free-form workout entry interface.
- Structured exercise and set summaries.
- Exercise-focused history and a progression chart.
- Session statistics/aggregate workload view.
- A clarification interaction for an ambiguous exercise name.

## Design trade-offs

- **Speed vs precision:** avoid making logging burdensome, but preserve the ability to correct mistakes.
- **Flexible input vs deterministic records:** users phrase exercises differently; stats need consistent identity.
- **Useful metrics vs noisy data:** historical corrections can alter records and progress calculations.
- **Feature breadth vs reliability:** a prototype should not promise untested platform coverage or finalized App Store behavior.

This file is a portfolio narrative of the actual development, not an indication of production release or validated usage/retention metrics.
