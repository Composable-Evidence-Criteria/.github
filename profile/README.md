# Recomputable Evidence

### Short Description
A shared test bench for checking whether separate specifications for AI agent evidence still hold up when they are used together.

### Scope of Lab
**The problem.** When an AI agent takes an action — makes a payment, calls a tool, acts for someone — several groups are now writing specifications for the record it leaves behind: who authorized it, what was done, who holds the keys. Each spec can be verified on its own. Real systems combine them: one spec records the authorization, another the payment, a third the custody of the keys. Few combinations have been checked, and each check was set up by one project under its own criteria. The typical failure is quiet: one record accepts another's claim of authority as if it were its own, and the result looks valid when it isn't. There is no shared set of criteria for judging a combination that the specs' maintainers wrote together.

**What the lab does.** It keeps two things in one neutral place:
- **Test cases** that pair records from two different specs and state the expected outcome, including cases that must fail. Anyone can rerun them offline from the published bytes: no hosted service, no account.
- **Criteria** for judging a combination, written jointly by the people who maintain the specs involved, not by any single author.

**What it does not do.** It does not pick a winning spec, does not certify anyone, and does not take over any spec. Each spec keeps its own repository and maintainers.