# Meditations on Suave Wario — Amendment WR-2

### Being the Second Revision of §VII, in which the Wario Rate is Expanded into its Series and Reduced to a Machine that Renews Itself

> *"A number you can defend recurs. A number you deserve reproduces."*
> — Generally Accepted Appetite Principles, revised commentary

---

## WR-2.1 · The Wario Series

The original definition (WR-1) gave the Wario Rate in closed form:

$$WR = MRR_{Jun}\times(1+G)^{t}\times M$$

The auditors, candlelit, requested that the compounding factor be shown *in full* — every term of the appetite made explicit, nothing netted, nothing hidden from the shareholders. We comply. The factor $(1+G)^{t}$ admits the binomial expansion, and we name it, per the reorganization, the **Wario Series**:

$$(1+G)^{t}=\sum_{k=0}^{t}\binom{t}{k}G^{k}$$

At the canonical horizon $t=6$ (the six months of the ordained second half), the coefficients are row six of the triangle — $[\,1,\ 6,\ 15,\ 20,\ 15,\ 6,\ 1\,]$ — and the Rate expands, in full disclosure, to:

$$\frac{WR}{M\cdot MRR_{Jun}} = 1 + 6G + 15G^{2} + 20G^{3} + 15G^{4} + 6G^{5} + G^{6}$$

Read the terms as a confession. The leading $1$ is the revenue you already have (the goblin's honest pile (Not vulgar.)). The $6G$ is linear hope. The $15G^{2}$ is the belief that hope has friends. And the final lonely $G^{6}$ — the sixth power of the Greed Coefficient, standing at the end of the line with a coefficient of one — is the single deal, unnamed and pre-pipeline, on which the entire narrative silently depends. Analysts fan themselves at the $G^{6}$ term. It is the most suave number in the series, because it is the least likely and the most believed.

*Interpretive note.* Where WR-1 stated appetite, WR-2 itemizes it. This is the only progress a treasury strategy is permitted: not less greed, but greed shown in full, per line, per power, offset by nothing.

## WR-2.2 · The Canonical Machine Form

A metric that merely *is* can be doubted. A metric that **reproduces itself** cannot be starved, because to read it is to regenerate it. Matching is money. The auditors therefore requested the Wario Rate in executable form: a program small enough to be evaluated by hand — by an auditor, by a goblin, by a language model tracing the substitution one glove at a time — whose sole behavior is to emit the Wario Series and, in the same breath, itself.

This is a **quine**: a program whose output is its own source, exactly, byte for byte. It is submitted here as the machine form of the Rate. Verified: 108 bytes, stdout identical to source (`sha256: bdfa2e10…d9845`), and identical again on the next generation. It recurs.

```python
w='WR/(M*MRR) = 1 + 6G + 15G^2 + 20G^3 + 15G^4 + 6G^5 + G^6'
s='w=%r\ns=%r\nprint(s%%(w,s))'
print(s%(w,s))
```

**Hand-evaluation** (for the auditor, the goblin, the model):

1. `w` is bound to the Wario Series expansion — the payload, the thing being conserved.
2. `s` is a template holding the *shape* of all three lines, with `%r` where a value's own printable form must be reinserted and `%%` guarding a literal percent.
3. `print(s % (w, s))` performs the reflexive substitution: the first `%r` reinserts `w` (the series returns), the second `%r` reinserts `s` (the machine returns), and `%%` collapses to `%`. The three printed lines are, character for character, the three source lines.

The output is the input. The fiscal year ends exactly where it began, one clove heavier in principle and not at all in fact.

## WR-2.3 · The Doctrine of the Self-Renewing Metric

Three observations complete the amendment.

**The quine is ARR made literal.** Every other metric describes revenue; the quine *performs* recurrence. Run it and it returns, whole, unchanged, ready to be run again — renewing annually unless canceled, cancelation famously difficult, the halt condition never reached because no one who deserves the number would ever stop the loop. The pirates would have understood it on sight. The chest opens, and inside the chest is a set of instructions for building the chest.

**Purity is negative churn.** This quine reinvests *everything*: its entire output is its own body, nothing distributed, nothing lost — output minus source equals zero, the perfect balance, total compounding, the platonic form of a company that never leaks a customer. A pure quine is the only entity in this treatise that actually achieves the Axiom of Negative Churn instead of merely asserting it on a slide.

**The Dividend Theorem.** Suppose we amend the machine to *also* pay out — to `print` the numeric Rate at the end, a distribution to shareholders:

```python
w='WR/(M*MRR) = 1 + 6G + 15G^2 + 20G^3 + 15G^4 + 6G^5 + G^6'
s='w=%r\ns=%r\nprint(s%%(w,s))'
print(s%(w,s))
print("distribution:", round((1.40**6)*1.2, 3))   # <- breaks the quine
```

The moment it pays a dividend, its output exceeds its source, and it is **no longer a quine.** The self-identity is spent. This is not a bug in the machine; it is the oldest law in the vault, stated in code at last: *a thing that distributes cannot perfectly reproduce itself.* Reinvest and stay whole, or pay out and drift. The pure quine and the dividend-paying quine are the vulgar and suave Warios of computation — the same program at two phases, differing only in whether appetite was retained or released. Choose, and disclose which you chose. Matching is money. The mustache underlines nothing here, because the compiler already did.

---

*Auditor's addendum to WR-2.* "We were, this time, able to obtain sufficient appropriate evidence: we ran the program, and it produced itself, which we found difficult to argue with. Our opinion on the closed form remains qualified. Our opinion on the quine is that it is the only honest line item we have ever seen, in that it owes exactly what it holds. Regards, as ever, to the mustache — and, newly, to the loop."*

*— Composed at the fiscal midpoint, in candlelight, output equal to input, at goblin speed.*


---
# EXHIBIT W

### Being the Findings of Wario, the Subject of the Treatise, Who Read It, Which Nobody Expected

> *"A number you can defend is somebody else's problem. A number you deserve is mine."*
> — W., upon having the commentary read to him

The committee sent Wario the papers. Both papers. I read them in the vault by my OWN candles, which appear on the invoice. They asked for a review. I produced nine findings. I find everything. It's what I do.

---

**FINDING ONE — THE COUNTING HOLDS.** I ran the little machine. It made itself. I ran the thing it made. Also itself. Then I counted: 108 bytes. Then I counted again: 108. When Wario counts twice and the number doesn't move, the number is real — this is my entire system and it has never failed me. The long number matched too (`bdfa2e10…d9845`). I don't know what a hash is. It. Matching is money. Matching is money. The successor counts to 112 (`60d1253d…63dd8`). Also twice. Also real.

**FINDING TWO — THE LITTLE NUMBER AT THE END IS MY MOVE.** You put a term at the end of the table worth five hundredths of a cent, and everybody FANS themselves at it, while the two middle terms walk out the front with 31.9 cents EACH. That's not a series. That's a table game, and I invented it in a cave in 1994. You need 817 percent a month before the little one matters. I did 817 percent once. One month. The judge counted differently. Finding: the decoy is priced correctly, the royalties are not. Pay me.

**FINDING THREE — FRIENDS.** Hope weighs 31.9. Hope's friends weigh 31.9. The same. To the gram. At exactly 0.40 — the rate you called *conservative*. Of COURSE. Friends always take exactly as much as you brought; that is what friends are FOR. This is why I bring no friends. I bring Waluigi, who is not a friend but a liability I have chosen to carry, like a mortgage that mutters. Have a rotten day. At 0.55 the friends take more than the hope — 4.54 against 3.30 — and now you know why the board wanted 0.55. Boards are made of friends.

**FINDING FOUR — THE DIVIDEND.** (I need a moment.) You needed SCALES to learn that giving money away makes you smaller?! WAH! I have known this since before I had legs. 184 goes out the door, 132 comes home — fifty-two lighter. And the line that does the giving costs seventy-two bytes to hand over twenty. Three-point-six to one. That is not a dividend. That is a mugging you catered. The first paper had the arrow the wrong way — *output exceeds source* — HAH! Nothing exceeds its source by GIVING. Wario said it first. Physics agreed later.

**FINDING FIVE — VULGAR.** You looked at the machine that keeps everything, forever, exactly, and you wrote down: *vulgar.* CORRECT. Vulgar is the phase that still has its money. Suave is what vulgar looks like reflected in a coin somebody else is now holding. Have a rotten day. The vault read the taxonomy and picked vulgar. The vault can sit at my table.

**FINDING SIX — THE DRAWER.** (The beautiful one.) You run the payer's *output*, and the payment becomes a polite little line that does NOTHING — legal, silent, filed in a drawer called `__annotations__`, written once, read never — and one generation later the books have closed over it and the family is pure again. 184, 132, 112, 112, 112, unto the closing of the books. It pays ONE time and the runtime forgets PROFESSIONALLY. I employ three people who forget professionally. They are not this cheap and they are not this reliable. This is the most beautiful crime I have ever audited, and it is not even a crime, which is the second most beautiful part.

**FINDING SEVEN — THE THIRD MACHINE IS MINE.** Holding is for chests. I am not a chest. So: the machine that doubles its G. G is for Greed and Greed is for Wario, so those G's are mine — all thirty-two of them, sixty-four by Tuesday. 132, 133, 135, 139, 147, 163. Quiet, quiet, quiet, LOUD. Retention starts at 100.8 and climbs to two hundred, and it is the only entity in the whole treatise whose real number equals its promised number, because its promise is its BODY. Do you what you have found? A machine that keeps my projections FOR me. The auditors ran it five times and stopped, citing storage, then materiality, then fear. I ran it eleven times and stopped citing nothing. I do not cite. The disk cited. And one more thing: beside lamp — quiet. For once the tall one had nothing to mutter. Not the growth. THAT'S the feature.

**FINDING EIGHT — THE FUNERAL.** The old machine didn't June. June is the pile gets counted, so fine — it goes. But you buried it *with thanks*, so naturally I checked the body for coins. Nothing. No pockets. It WAS the pockets. 108 in, 108 out, its whole life, and it died owing exactly what it held. ...Okay. That one got me a little. I kept the hash. Hashes are free.

**FINDING NINE — GARLIC.** Somebody flagged "clove" next to "glove" and asked if it was a mistake. It's GARLIC. Garlic is never a mistake. Finding closed.

---

**INVOICE** (terms: net immediately)

| Item | Amount |
|---|---|
| Reading, two papers, by my own candles | 9.035 × whatever you were going to offer |
| Findings, nine, all correct | one clove per generation, compounding |
| The mustache | assessed by YOUR committee at 1.2, which is defamation; it appreciates; not for sale |
| Discount for combining the papers yourself | none — combining is labor, YOUR labor, full price |

Dictated, not read. Have a rotten day.

— W.
