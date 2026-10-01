# AI Automation vs. Legacy APIs

### The Hidden Contracts Behind "The API Broke"

**Sean Murray** · ~10–12 min · 2026

## The problem

You connect AI automation to a business system through its API. Every call returns `200 OK`. The records look fine — and are quietly wrong (pricing, taxes, follow-on steps that never ran). By morning someone says: *"the API broke."*

It usually didn’t. What broke was a **hidden contract**: a rule about meaning, sequence, identity, or retries that nobody wrote down, and that a human used to fulfil by clicking through the UI. This talk explains that model and one fix: give the AI a **single safe verb** that keeps those promises (`create_confirmed_thing`), not the raw create endpoint.

## Who it helps

- Engineers wiring AI into ERPs / CRMs / “legacy” APIs  
- Ops people who hear “the API broke” and need a clearer diagnosis  
- Anyone who missed the talk and still wants the argument in plain language  

## How to run / browse

No install for the slides.

1. **Missed the room?** Start with [Remarks](./REMARKS.md) (full argument in prose).  
2. Then open [`Hidden_Contracts_Slides.html`](./Hidden_Contracts_Slides.html) in a browser (example panels animate).  
3. PDF fallback: [`Hidden_Contracts_Slides.pdf`](./Hidden_Contracts_Slides.pdf) if present in this folder.

```bash
open Hidden_Contracts_Slides.html
```

| Asset | What it is |
|---|---|
| [`Hidden_Contracts_Slides.html`](./Hidden_Contracts_Slides.html) | Deck (preferred) |
| [`REMARKS.md`](./REMARKS.md) | Standalone write-up |
| [`One_Pager.html`](./One_Pager.html) | One-page summary |

## Key lines

- "A 200 OK is the most dangerous thing the AI can hear."
- "All five can return 200 OK while being wrong."
- "'The API broke' is a review comment about your system, not the model's."

Examples are **vendor-neutral** (no employer or product names) so the lesson travels to any business system.
