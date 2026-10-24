<div align="center">
<img src="assets/portrait-240.jpg" width="132" alt="Emmanuel Agama">
<h1>Emmanuel Agama</h1>
<p>Independent AI evaluation · Abuja, Nigeria</p>
<p><a href="https://agamanexus.com">agamanexus.com</a> &nbsp;·&nbsp; <a href="mailto:emmanuel@agamanexus.com">Email</a> &nbsp;·&nbsp; <a href="https://linkedin.com/in/emmanuelagama">LinkedIn</a> &nbsp;·&nbsp; <a href="https://emmyagama.substack.com/">Substack</a></p>
</div>

---

I measure whether AI systems answer correctly, and I publish the measurements even when they are unflattering.

Most AI vendors show a demo. A demo proves an answer can exist; it does not tell you how often the answer is wrong. The work here is the other thing: build a fixed test set, run the system against it honestly, count the failures by class, and put the weak number on the same page as the good ones.

## The work behind everything else

**[ng-health-reg-assistant](https://github.com/emmyagama/ng-health-reg-assistant)** — a question-answering assistant over eight public Nigerian health-regulation PDFs. It cites the document and section behind every claim, refuses when the corpus cannot answer, and blocks clinical questions outright.

Fifty hand-built questions. Twenty-five answerable, twenty-five deliberately not. The raw model invented answers twice; the guardrails caught both, which is why the published hallucination rate is 0.000 rather than 0.000-on-the-shown-surface-only. Retrieval is the weak layer at recall@5 **0.379**, and that number is on the front of the README, not in an appendix.

Every published figure regenerates from a committed run, and one command checks the README against it. The method is written up for a non-specialist at [agamanexus.com/notes/how-i-measured-a-health-regulation-assistant](https://agamanexus.com/notes/how-i-measured-a-health-regulation-assistant/).

## How I work

| | |
|---|---|
| **Measurement before claims** | A number in a document must point at a file in a repository. If it cannot, it does not ship. |
| **Failures are counted, not averaged away** | A wrong answer is attributed to the layer that caused it and keyed to a question id, so a fix can be falsifiable. |
| **One named person** | The person who measures your system is the person who signs the report. No account managers, no handoffs. |
| **No compliance claims** | I produce evidence. Your counsel interprets it. I do not promise that anything will pass. |

## Selected repositories

| Repository | What it is |
|---|---|
| **[ng-health-reg-assistant](https://github.com/emmyagama/ng-health-reg-assistant)** | Retrieval + guardrail evaluation over Nigerian health-regulation documents. Versioned, reproducible, CI-checked. |
| **[proposalos](https://github.com/emmyagama/proposalos)** | Proposal generation tooling. |
| **[portfolio](https://github.com/emmyagama/portfolio)** | Earlier site work, kept for reference. |

<sub>Everything else here is exploration, prototypes and work in progress. Repositories are not curated to look impressive — the pinned ones are the ones I would defend.</sub>

## Elsewhere

- **Site** — [agamanexus.com](https://agamanexus.com)
- **Method note** — [how I measured a health-regulation assistant](https://agamanexus.com/notes/how-i-measured-a-health-regulation-assistant/)
- **Writing** — [The Digital South Journal](https://emmyagama.substack.com/) on efficiency-first infrastructure in emerging markets
- **Contact** — [emmanuel@agamanexus.com](mailto:emmanuel@agamanexus.com)

<sub>Abuja, Nigeria · WAT (UTC+1) · Open to paid AI evaluation work — fixed price, fixed dates.</sub>
