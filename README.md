## Abhishek Sharma

Staff engineer, distributed systems and money movement. I work on the correctness
problems that only appear under retry, partial failure and concurrency — the class
of bug whose symptom is a customer charged twice.

### Open source

<table>
  <thead>
    <tr>
      <th rowspan="2" align="left">Project</th>
      <th rowspan="2" align="right">Stars</th>
      <th colspan="3" align="center">My contributions</th>
    </tr>
    <tr>
      <th align="center">Bug fixes</th>
      <th align="center">Features &amp; docs</th>
      <th align="center">Reviews</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="https://github.com/addyosmani/agent-skills">addyosmani/agent-skills</a></td>
      <td align="right">~92k</td>
      <td align="center"><a href="https://github.com/addyosmani/agent-skills/pulls?q=author%3Aabhisheksharma2411"><b>1</b> + 2</a></td>
      <td align="center"><a href="https://github.com/addyosmani/agent-skills/pulls?q=author%3Aabhisheksharma2411"><b>1</b> + 1</a></td>
      <td align="center"><a href="https://github.com/addyosmani/agent-skills/pulls?q=reviewed-by%3Aabhisheksharma2411+-author%3Aabhisheksharma2411">6</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/diegosouzapw/OmniRoute">diegosouzapw/OmniRoute</a></td>
      <td align="right">~60k</td>
      <td align="center"><a href="https://github.com/diegosouzapw/OmniRoute/pulls?q=author%3Aabhisheksharma2411"><b>4</b> + 1</a></td>
      <td align="center">—</td>
      <td align="center"><a href="https://github.com/diegosouzapw/OmniRoute/pulls?q=reviewed-by%3Aabhisheksharma2411+-author%3Aabhisheksharma2411">7</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/juspay/hyperswitch">juspay/hyperswitch</a></td>
      <td align="right">~44k</td>
      <td align="center"><a href="https://github.com/juspay/hyperswitch/pulls?q=author%3Aabhisheksharma2411">2</a></td>
      <td align="center"><a href="https://github.com/juspay/hyperswitch/pulls?q=author%3Aabhisheksharma2411">2</a></td>
      <td align="center"><a href="https://github.com/juspay/hyperswitch/pulls?q=reviewed-by%3Aabhisheksharma2411+-author%3Aabhisheksharma2411">6</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/goauthentik/authentik">goauthentik/authentik</a></td>
      <td align="right">~25k</td>
      <td align="center"><a href="https://github.com/goauthentik/authentik/pulls?q=author%3Aabhisheksharma2411"><b>4</b> + 1</a></td>
      <td align="center"><a href="https://github.com/goauthentik/authentik/pulls?q=author%3Aabhisheksharma2411"><b>1</b> + 1</a></td>
      <td align="center"><a href="https://github.com/goauthentik/authentik/pulls?q=reviewed-by%3Aabhisheksharma2411+-author%3Aabhisheksharma2411">7</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/lidge-jun/opencodex">lidge-jun/opencodex</a></td>
      <td align="right">~13k</td>
      <td align="center"><a href="https://github.com/lidge-jun/opencodex/pulls?q=author%3Aabhisheksharma2411"><b>2</b></a></td>
      <td align="center"><a href="https://github.com/lidge-jun/opencodex/pulls?q=author%3Aabhisheksharma2411">1</a></td>
      <td align="center"><a href="https://github.com/lidge-jun/opencodex/pulls?q=reviewed-by%3Aabhisheksharma2411+-author%3Aabhisheksharma2411">7</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/akitaonrails/ai-memory">akitaonrails/ai-memory</a></td>
      <td align="right">~5k</td>
      <td align="center"><a href="https://github.com/akitaonrails/ai-memory/pulls?q=author%3Aabhisheksharma2411"><b>2</b></a></td>
      <td align="center">—</td>
      <td align="center"><a href="https://github.com/akitaonrails/ai-memory/pulls?q=reviewed-by%3Aabhisheksharma2411+-author%3Aabhisheksharma2411">5</a></td>
    </tr>
    <tr>
      <td align="right"><b>Total</b></td>
      <td align="right"><b>~239k</b></td>
      <td align="center"><b>13</b> + 6</td>
      <td align="center"><b>2</b> + 5</td>
      <td align="center"><b>38</b></td>
    </tr>
  </tbody>
</table>

<sub><b>Bold</b> = merged; plain = open, under review. Counts link through to the pull requests.</sub>

Merged by those projects' own maintainers — [`addyosmani`](https://github.com/addyosmani),
[`diegosouzapw`](https://github.com/diegosouzapw) (OmniRoute lead),
[`akitaonrails`](https://github.com/akitaonrails) (ai-memory lead),
[`BeryJu`](https://github.com/BeryJu) (authentik lead), [`rissson`](https://github.com/rissson),
[`dominic-r`](https://github.com/dominic-r), [`lidge-jun`](https://github.com/lidge-jun)
and [`Wibias`](https://github.com/Wibias).

Alongside the pull requests, **38 reviews** on other contributors' work across the
six projects — usually the more useful half. A representative one: on an OmniRoute
combo-routing fix I traced a persisted routing pin back through both of its readers
and flagged that clearing it unconditionally would discard a healthy provider. That
review outlived the pull request it was left on, and the finding became its own
change once I could measure which routing strategy it actually affected.

### My projects

**[justonce](https://github.com/abhisheksharma2411/justonce)** · [PyPI](https://pypi.org/project/justonce/) — make side effects happen exactly once. Idempotency keys, atomic claims, divergence detection and reconciliation for Python, with SQLite, Postgres and Django stores held to one shared conformance suite.

**[distributed-systems-skills](https://github.com/abhisheksharma2411/distributed-systems-skills)** — agent skills for production correctness: exactly-once semantics, and failure-mode analysis before the happy path is written.

**[retry-safe-payment-idempotency-artifact](https://github.com/abhisheksharma2411/retry-safe-payment-idempotency-artifact)** — a bounded TLA+ model and deterministic conformance artifact for retry-safe payments.

---

*The `authentik`, `hyperswitch`, `opencodex`, `agent-skills`, `OmniRoute` and
`ai-memory` repositories under this account are forks, kept only because GitHub
requires one to open a pull request. A fork carries none of the upstream project's
stars; the contributions are the pull requests above.*
