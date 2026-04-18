# Investor Paths — Legal Scaffolding Notes

*Working notes for Ryan + Mike + legal counsel. Not legal advice. Must be reviewed by a securities attorney before any capital is accepted.*

Last updated: 2026-04-18

---

## TL;DR — The Three Paths Summary

| Path | Structure | Wrapper | Minimum | Target Investor |
|---|---|---|---|---|
| **Founders' Circle** | Classic SAFE | Reg D 506(c) | $25K | Accredited only |
| **Flywheel Fund** | Revenue share units | Reg CF (up to $5M/yr) | $500 | Anyone (with limits) |
| **Compound Path** | Monthly-contribution SAFE | Reg CF for <$1K/mo tiers; Reg D 506(c) for $1K+/mo tiers | $100/mo | Anyone (non-accred. via Reg CF) |

---

## Path 1 — Founders' Circle (Traditional SAFE)

**This is the easy one. Ship it first.**

### Structure
- Standard YC-style SAFE (Simple Agreement for Future Equity).
- **Valuation cap:** $8M (proposed — anchor against current traction).
- **Discount:** 20% to next priced round.
- **Minimum:** $25K.
- **Pro-rata rights:** Yes, for checks $50K+.

### Regulatory wrapper — Reg D 506(c)
- Allows **general solicitation** (i.e., we can publicly advertise on invest.html and social media).
- **All investors must be accredited.** (Income >$200K/yr solo or $300K joint for 2+ years, OR net worth >$1M excluding primary residence.)
- Liftori must take **reasonable steps to verify accreditation** — accepted methods: investor provides CPA letter, W-2s/tax returns, or uses a third-party verification service (e.g., VerifyInvestor.com, Parallel Markets).
- **Form D** must be filed with SEC within 15 days of first sale.
- State "blue sky" notice filings in each investor's state of residence.

### Documents needed
1. SAFE agreement (YC template, lightly customized)
2. Subscription agreement
3. Accredited investor verification form
4. Privacy policy + terms of service
5. Form D
6. Cap table (add SAFE holders in "side pocket" — they convert at next priced round)

### Estimated legal cost
**$3,000 – $7,000** for a simple 506(c) setup with a reasonable securities attorney. Clerky, Stripe Atlas, or direct engagement with a startup-focused lawyer (recommended: any YC-network-affiliated firm).

---

## Path 2 — Flywheel Fund (Revenue Share)

**This is the creative one. Requires more legal work, but also differentiates us massively.**

### Structure options (discuss with lawyer — pick one)

**Option A — Revenue Share Agreement (RSA) [simpler]**
- Each investor signs an RSA that entitles them to a **percentage of Liftori's defined "Platform Fee Revenue"** (narrowly defined as the processor markup collected on client GMV).
- Investor receives pro-rata monthly distributions of that revenue pool.
- **Not equity.** Investor has no voting rights, no conversion into equity.
- **Recommendation:** Easier to set up. Closer to a TinySeed / Earnest Capital structure.

**Option B — Tokenized Revenue Share Units [disruptor play]**
- Same underlying mechanics as RSA, but units are issued as **digital securities** (security tokens) on a compliant platform like Republic Crypto or Securitize.
- Secondary trading becomes possible after a 12-month hold (Reg CF restriction).
- **Recommendation:** Higher setup cost, but creates massive PR story — "first AI-native SMB platform to tokenize revenue share."

### Regulatory wrapper — Reg CF
- **Maximum raise:** $5M per 12-month period.
- **Non-accredited investors allowed** with individual investment limits based on income/net worth.
- **Must use a registered funding portal:** Wefunder, Republic, StartEngine are the dominant options. They handle compliance, investor onboarding, escrow, and filings.
- **Form C** filed with SEC before launch.
- **Financial statements required:** For raises >$1.07M, we need CPA-reviewed financials. Under $1.07M, unreviewed is fine. (Since we're pre-revenue, review costs ~$5K-$10K.)
- **Offering page** on the funding portal must include risk disclosures, use of proceeds, cap table, and quarterly updates to investors during the raise.

### Documents needed
1. Revenue Share Agreement (RSA) OR digital security offering memorandum
2. Escrow agreement with funding portal
3. Form C + risk disclosures
4. Offering page content
5. Defined methodology for calculating "Platform Fee Revenue" (this is the most important — must be auditable and transparent)
6. Monthly distribution mechanics + wallet/bank setup

### Estimated legal + portal cost
- **Legal:** $10,000 – $20,000 for initial structuring (RSA drafting, Form C prep, offering memo).
- **Portal fee:** Wefunder takes ~7.5% of raised capital. Republic takes ~6%.
- **CPA review:** $5K – $10K.
- **Total:** Budget **$25K – $40K** all-in to launch the Flywheel Fund raise.

### The trade-off
High upfront cost, but the Flywheel Fund is the vehicle that can raise $500K – $5M from the widest investor base. ROI is excellent if we hit even 20% of our fundraising target.

---

## Path 3 — Compound Path (Monthly SAFE Drip)

**This is the disruptor. Most technically novel — we'll be one of the first companies to do this.**

### Core legal question
> *Can a single SAFE agreement legally bind monthly recurring contributions at a locked valuation cap?*

Answer: **Yes, with proper structuring.** It's essentially a "master SAFE + contribution schedule" arrangement. Each monthly contribution is treated as a separate securities purchase, but all are governed by the same cap table treatment. Needs a lawyer to draft the "Recurring Contribution Rider" correctly.

### Structure
- **Master SAFE agreement** signed once at enrollment.
- **Recurring Contribution Rider** specifies: monthly amount, duration (12 months default), locked valuation cap ($8M), ACH authorization.
- Each monthly ACH debit is a **separate securities purchase** under the master SAFE, at the same cap.
- At the end of 12 months, investor has contributed $N (e.g., $3,000 at $250/mo) and holds SAFE rights for that aggregate amount.
- SAFE converts to equity at next priced round or liquidity event, same as Founders' Circle.

### Regulatory wrapper — split by tier
- **$100/mo, $250/mo, $500/mo tiers (non-accredited-friendly):** Reg CF. Use the same funding portal as the Flywheel Fund (Wefunder or Republic). This folds nicely into the Reg CF raise.
- **$1,000/mo and $2,500/mo tiers (accredited-friendly):** Reg D 506(c). Same infrastructure as Founders' Circle.

### Key compliance wrinkles
1. **ACH processing:** Need a payment processor that handles recurring micro-debits (Stripe, Plaid, or Dwolla). Must comply with NACHA rules for recurring authorization.
2. **Monthly contribution as "separate sale":** Each debit triggers a separate securities purchase. State blue sky filings must accommodate cumulative sales volume.
3. **Cancellation mechanics:** Investor must be able to cancel recurring debits at any time. We must process cancellation within 3 business days (Reg E rules for consumer ACH).
4. **Accreditation re-verification:** For Reg D tiers, accreditation must be verified every 5 years (or at substantial new subscription changes).
5. **Reg CF investor limits:** Non-accredited investors have annual investment limits across all Reg CF offerings. Portal handles this automatically.

### Documents needed
1. Master SAFE with Recurring Contribution Rider
2. ACH authorization form (NACHA-compliant)
3. Per-tier subscription addendum
4. Cancellation policy
5. Annual recap statement (investor needs to see total position at year-end)
6. All the Reg CF + Reg D docs from Paths 1 and 2

### Estimated legal cost
**$5,000 – $10,000** **on top of** Paths 1 and 2 — the heavy lifting is the Recurring Contribution Rider + ACH compliance. Everything else is reusable.

---

## Total Legal Budget Estimate

| Item | Low | High |
|---|---|---|
| Path 1 (Founders' Circle) | $3K | $7K |
| Path 2 (Flywheel Fund) | $25K | $40K |
| Path 3 (Compound Path) incremental | $5K | $10K |
| CPA review + bookkeeping cleanup | $5K | $10K |
| Contingency / filings | $2K | $5K |
| **TOTAL** | **$40K** | **$72K** |

That's the worst-case all-in to launch all three paths **legally and SEC-compliantly**.

---

## Phased Rollout Recommendation

Rather than launching all three simultaneously, ship in phases to manage legal spend + cash flow:

### Phase A (Now → 30 days): Founders' Circle only
- Cheapest to set up ($3K–$7K).
- Accredited-only, so no Reg CF portal dependency.
- We can start raising $25K+ checks immediately while lawyers work on Paths 2 and 3.
- **Target raise from Phase A:** $200K–$500K.

### Phase B (Days 30–90): Compound Path launch
- Layer on top of the existing SAFE infrastructure.
- Soft-launch the $1K+/mo Reg D tiers first (no portal needed).
- Public launch the $100–$500/mo Reg CF tiers via Wefunder/Republic once portal is live.
- **Target raise from Phase B:** $150K–$500K.

### Phase C (Days 90–180): Flywheel Fund launch
- The biggest raise, most complex setup.
- Use CPA-reviewed financials from Phase A traction as proof.
- Run a dedicated Reg CF campaign on the chosen portal (Wefunder recommended for its "subscription-style" investor base).
- **Target raise from Phase C:** $500K–$2M.

---

## Open Questions for Legal Counsel

Queue these up for the first attorney meeting:

1. **Entity structure:** Does Liftori, LLC need to convert to a Delaware C-Corp before issuing SAFEs? (Likely yes for SAFE-based raises — YC SAFE template assumes C-Corp.)
2. **Flywheel Fund:** RSA vs. tokenized security — which does the lawyer prefer from a regulatory clarity standpoint?
3. **Compound Path recurring rider:** Is there precedent for this structure? What's the cleanest Master SAFE template to adapt?
4. **State blue sky filings:** How do we handle multi-state investors without triggering costly state-by-state filings? (Reg CF and Reg D 506(c) largely preempt state registration, but notice filings still apply in most states.)
5. **Investor reporting cadence:** What's the minimum disclosure cadence required post-raise for each wrapper?
6. **Marketing copy:** Our "revolutionary" positioning on invest.html — is there anything that needs a disclaimer rewrite to avoid being a misleading statement?
7. **Anti-money-laundering (AML):** For Reg CF, the portal handles KYC/AML. For Reg D direct sales, we need our own process. What's the MVP?

---

## Recommended Legal Partners

Not an endorsement — just starting points to vet:

- **Gunderson Dettmer** — YC-aligned, expensive but gold standard.
- **Wilson Sonsini** — similar tier.
- **Clerky** — fixed-price SAFE + 506(c) packages ($2K–$5K). Budget option for Phase A.
- **Cooley GO** — free templates + paid review. Good middle-tier option.
- **Republic / Wefunder** — both provide in-house or referred legal counsel as part of their funding portal services. Lowers the Reg CF legal lift significantly.

My recommendation: **Start with Clerky for Phase A** (fast, cheap, good enough for a $25K SAFE) → **engage Republic's legal team for Phase B/C** when we're ready for Reg CF.

---

## Next Steps for Ryan + Mike

1. **Confirm entity structure.** Liftori, LLC is in formation. Decide now: stay LLC and use a simple profit-share for Flywheel Fund, or convert to Delaware C-Corp to enable SAFE + Reg CF.
2. **Book 30-min intro calls with 2 lawyers.** Use this doc as the brief.
3. **Pre-select funding portal.** Wefunder vs. Republic — different investor demographics. Mike should pick based on which investor base matches our pitch better.
4. **Set Phase A target close date.** Aim for 30 days from today → first SAFE signed by ~2026-05-18.
5. **Track every conversation with potential Phase A investors now** — when the paper is ready, we want a queue lined up.
