# Prototype: Juno Insights

**Link:** https://claude.ai/artifact/Cz1ZGpYGKkjZptXqNYj7NN

## The problem
A PM collects customer feedback from many places. The same request shows up several times, risky requests (renewals, security, competitors) sit next to nice-to-haves, and it is hard to see what belongs on the roadmap.

## What the prototype demonstrates

**Feedback tab**
- Groups similar requests as **possible duplicates**, with Merge (customers combine) and Not duplicates.
- Sorts the rest into **possible risks**, **possible quick wins** (medium or high impact, small effort), **possible low priorities** (low impact, fewer than 3 customers) and everything else.
- Shows why a request is flagged as a risk, for example "renewal, security, SSO".
- Lets the PM add new feedback, which is sorted immediately, and add any request to a quarter.

**Roadmap tab**
- Quarterly columns (Q4 2026 to Q3 2027) and five swimlanes: Onboarding, Reporting, Integrations, Mobile, Security & Admin.
- A star on every roadmap item that has customer feedback attached, with the number of customers who asked.
- Selecting an item shows the feedback and customers behind it. Items can be moved between quarters or removed.
- "Fill from feedback" proposes quarters from risk and effort, and skips low priorities and unresolved duplicates.

All customers and requests are made-up examples. Changes are saved in the viewer's own browser only.

## Debrief

**What worked**
- Putting duplicates first makes the other lists cleaner, because merging combines customer counts before anything is prioritized.
- The star and customer count make it clear which roadmap items are backed by customers and which are not.

**Limits**
- Sorting is rule-based, not AI. Duplicates use word overlap and risks use a keyword list, so paraphrased duplicates can be missed and a keyword can flag a request that is not really a risk.
- Impact and effort are entered by hand. The prototype does not estimate them.
- Data is not shared across people or devices, and nothing is imported from real sources such as support tickets, a CRM or call notes.

**Next steps**
- Use a language model to find duplicates by meaning and to summarize each group.
- Import feedback from a CSV or connected tools.
- Add a human-review step before any merge or roadmap placement, and measure how often the PM overrides the suggestions.
