# Sample Flight Check report

This is what Flight Check produces when run on a real deck. The deck below contains intentional issues so you can see what each finding type looks like.

---

## The input deck

> **SLIDE 1 — Q3 Market Overview**
> In today's fast-paced world, our strategic initiatives have leveraged comprehensive market analysis to deliver robust outcomes for our stakeholders. We delved into the customer journey to identify significant growth opportunities.
>
> **SLIDE 2 — Key Findings**
> — Strong performance across all segments
> — The customer base expanded considerably
> — Various improvements were implemented
> — Total revenue: $4.2B in Q3 (up from $3.8b in Q2)
> — McKinsey Global Institute (2023) found that 73% of CFOs prioritize this
>
> **SLIDE 3 — Customer Segmentation**
> Our analysis reveals three distinct customer cohorts driving substantial value. The first segment, comprising 40% of revenue, demonstrates strong engagement metrics. The second segment accounts for 30% of revenue. The third represents the remaining 35%.
>
> **SLIDE 4 — Recommendation**
> We recommend significant investment in segment one to harness untapped potential and unlock new revenue streams. This positions us well moving forward in an increasingly complex landscape.
>
> **SLIDE 5 — Financial Projections**
> Pipeline grew to $4.2 billion in Q3 — a substantial increase. Revenue projections for Q4 indicate strong continued growth across all key metrics. Citation: Bloomberg Industry Report, "Future of Enterprise Tech," 2024.

---

## The Flight Check output

### Flight Check: Q3 Market Overview Deck

#### Critical issues (fix before sending)

- **Slide 3, "Customer Segmentation":** Segmentation percentages sum to **105%**, not 100% (40% + 30% + 35%). This is the number that will get called out in the room.
- **Slide 2, "Key Findings":** Inconsistent unit formatting — *"$4.2B in Q3 (up from $3.8b in Q2)"*. Capital B and lowercase b mixed in the same line.
- **Slide 2, "Key Findings":** Citation *"McKinsey Global Institute (2023) found that 73% of CFOs prioritize this"* — verify this specific report exists. The Global Institute is real, but AI fabricates plausible-sounding McKinsey reports constantly. If you can't find this study in MGI's public catalog, the number is suspect.
- **Slide 5, "Financial Projections":** Citation *"Bloomberg Industry Report, 'Future of Enterprise Tech,' 2024"* — verify before sending. The report title is generic enough to be fabricated.

#### High-priority issues (fix if time allows)

- **Slide 1, title:** "Q3 Market Overview" is a topic label, not a finding. What's the message of the slide? *Example rewrite: "Q3 revenue grew on the strength of three segments — but one is at risk."*
- **Slide 1, body:** *"In today's fast-paced world"* — stock AI opener. Cut it; nothing else in the sentence depends on it.
- **Slide 1, body:** *"leveraged comprehensive market analysis"* — both "leveraged" and "comprehensive" are AI-pattern words. The sentence works without them.
- **Slide 1, body:** *"delved into the customer journey"* — "delved" is currently the most-recognized AI tell on the internet. Replace with "studied" or "mapped."
- **Slide 1, body:** *"stakeholders"* — name them. Who specifically? Customers, the board, regulators?
- **Slide 2, bullet 1:** *"Strong performance across all segments"* — adjective hiding a number. What growth rate? Across which segments?
- **Slide 2, bullet 2:** *"The customer base expanded considerably"* — by how much? Which customer base?
- **Slide 2, bullet 3:** *"Various improvements were implemented"* — vague catch-all. List them, or cut the bullet.
- **Slide 4, body:** *"significant investment"* — how much? In dollars or as a percentage of budget?
- **Slide 4, body:** *"harness untapped potential and unlock new revenue streams"* — three AI-pattern verbs in one phrase. Rewrite as a specific mechanism.
- **Slide 4, body:** *"moving forward in an increasingly complex landscape"* — filler. Cut.

#### Polish issues (catch on a final read)

- Em-dashes used as connective tissue on most slides — vary punctuation or break into shorter sentences.
- Slide titles 2, 3, 4, 5 are all noun phrases ("Key Findings," "Customer Segmentation," etc.). Read only the titles in order — do they tell the story? Currently they don't.
- Slide 3 mentions "strong engagement metrics" without showing the metric. Either show the number or drop the claim.

#### What's working

- The deck has a clear three-act structure: market view → segmentation → recommendation. The bones are good.
- Real quarterly comparison attempted on slide 2 ($4.2B vs $3.8B). Format inconsistency aside, the comparison is the right kind of evidence.
- Slide 4 makes an actual recommendation rather than just describing options.

#### Suggested next step

Fix the segmentation math on slide 3. That single error is the one that will get called out in the room and undermine everything else in the deck.

---

## Notes on this output

- Every flagged item quotes the **exact text** from the deck, so you can find it instantly.
- Items are organized by **severity**, not slide number — what could break the presentation comes first.
- "What's working" exists so you know which patterns to keep, not to soften the critique.
- Citations are flagged for **manual verification** rather than confirmed-fake. The skill can't verify against external databases — that's a Tier 3 feature for a future version. For now, it flags suspicious patterns so you can check yourself.
