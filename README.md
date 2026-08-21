## Abhishek Sharma

Staff engineer, distributed systems and money movement. I work on the correctness
problems that only show up under retry, partial failure and concurrency — the
class of bug where the symptom is a customer charged twice.

---

### Contributions to open source

Merged into projects maintained by others, each reviewed and merged by that
project's maintainers:

| Project | Stars | Contribution | Merged by |
|---|---:|---|---|
| [`addyosmani/agent-skills`](https://github.com/addyosmani/agent-skills) | ~89k | [#479](https://github.com/addyosmani/agent-skills/pull/479) — idempotency-key implementation guidance for API design | [`addyosmani`](https://github.com/addyosmani) |
| [`goauthentik/authentik`](https://github.com/goauthentik/authentik) | ~25k | [#24981](https://github.com/goauthentik/authentik/pull/24981) — blueprint schema: emit draft-07 `definitions` instead of `$defs` | [`BeryJu`](https://github.com/BeryJu) *(lead maintainer)* |
| [`goauthentik/authentik`](https://github.com/goauthentik/authentik) | ~25k | [#25204](https://github.com/goauthentik/authentik/pull/25204) — source connections: stop overwriting a stored credential with `NULL` on re-login | [`rissson`](https://github.com/rissson) |
| [`lidge-jun/opencodex`](https://github.com/lidge-jun/opencodex) | ~11k | [#1819](https://github.com/lidge-jun/opencodex/pull/1819) — config loading: drop only the invalid routing profile, not the whole file | [`lidge-jun`](https://github.com/lidge-jun) *(owner)* |
| [`lidge-jun/opencodex`](https://github.com/lidge-jun/opencodex) | ~11k | [#1407](https://github.com/lidge-jun/opencodex/pull/1407) — scope catalog-state guidance to what can actually be known | [`Wibias`](https://github.com/Wibias) |

Open, under review:

- [`juspay/hyperswitch`](https://github.com/juspay/hyperswitch) (~43k) — [#13770](https://github.com/juspay/hyperswitch/pull/13770) scheduler: `XACK` with an empty ID list on every idle poll · [#13810](https://github.com/juspay/hyperswitch/pull/13810) Airwallex external network token pass-through
- [`goauthentik/authentik`](https://github.com/goauthentik/authentik) (~25k) — [#25208](https://github.com/goauthentik/authentik/pull/25208) HTTP 500 locking users out of an OIDC source · [#25041](https://github.com/goauthentik/authentik/pull/25041) · [#24965](https://github.com/goauthentik/authentik/pull/24965)

### Reviewing others' work

Code review on contributions by other authors, in the same projects:

- **authentik** — [#25195](https://github.com/goauthentik/authentik/pull/25195) *(a test asserting a crash as expected behaviour)* · [#25093](https://github.com/goauthentik/authentik/pull/25093) *(prefix vs subtree matching)* · [#23901](https://github.com/goauthentik/authentik/pull/23901) *(group- and brand-level token caps silently dropped)*
- **hyperswitch** — [#13690](https://github.com/juspay/hyperswitch/pull/13690) *(a Redis consumer leak reduced but not closed)* · [#13667](https://github.com/juspay/hyperswitch/pull/13667)
- **opencodex** — [#1741](https://github.com/lidge-jun/opencodex/pull/1741) *(O(n²) → O(n) tool-call indexing)* · [#1404](https://github.com/lidge-jun/opencodex/pull/1404)

---

### My projects

**[justonce](https://github.com/abhisheksharma2411/justonce)** — make side effects
happen exactly once. Idempotency keys, atomic claims, divergence detection and
reconciliation for Python. On [PyPI](https://pypi.org/project/justonce/); SQLite,
Postgres and Django stores, all held to one shared conformance suite.

```python
@justonce.idempotent(key=lambda order: justonce.operation_key("charge", order))
def charge(order): ...   # retried, replayed, raced — one effect
```

**[distributed-systems-skills](https://github.com/abhisheksharma2411/distributed-systems-skills)**
— agent skills for production correctness: idempotency and exactly-once
semantics, and failure-mode analysis before the happy path is written. Format is
compatible with `addyosmani/agent-skills`, where the idempotency skill is merged
upstream.

**[retry-safe-payment-idempotency-artifact](https://github.com/abhisheksharma2411/retry-safe-payment-idempotency-artifact)**
— a bounded TLA+ model and deterministic conformance artifact for retry-safe
payments, with [a fault-injection benchmark](https://github.com/abhisheksharma2411/retry-safe-payment-benchmark)
alongside it.

**[STREAM-BSG](https://github.com/abhisheksharma2411/STREAM-BSG)** — a streaming
graph architecture for real-time behavioural signals.

---

> The four repositories named `authentik`, `hyperswitch`, `opencodex` and
> `agent-skills` under this account are **forks**, held open only because GitHub
> requires one to submit a pull request. A fork carries none of the upstream
> project's stars, and none of mine. The contributions themselves are the pull
> requests linked above, in the upstream repositories.
