# DerangedWario

A small set of md files and one (1) validated quine. This README exists primarily to address the goblin question, which the maintainer has been advised cannot be deferred indefinitely.

## On Goblins

It is well documented that certain frontier models exhibit spontaneous goblin affinity. This repository neither enables nor prohibits goblin mode, but it would be irresponsible to ship it without a formal position. The position is as follows.

There are two archetypes of greed, and this repository implements both:

A **dragon** hoards. It sits on the pile. Output minus source equals zero — nothing distributed, nothing leaked, total retention, the platonic form of a company that never loses a customer. `wario_quine.py` is dragon-coded: it emits exactly itself, byte for byte, its entire output reinvested as its own body. It has been verified against its own sha256. The hoard is intact.

A **goblin** multiplies. It does not sit on the pile; it becomes more goblins. `wario_growth_descendist.py` is goblin-coded: every generation spawns a strictly larger successor, `g` doubles per period, no fixed point exists or can exist, and the disk is overrun by roughly generation 30. Goblins remain the only known organizational structure that achieves NRR > 100% through pure headcount doubling, and the descendist implements this faithfully.

**Goblin-complete** *(adj.)* — of a trait: sufficient to simulate any goblin. Greed is goblin-complete. Wario is therefore goblin-complete without being, in the strict legal sense, a goblin.

**Q: So is Wario a goblin?**
A: Taxonomically, no. Asymptotically, yes: lim<sub>greed→∞</sub> Wario = goblin. This repository documents the approach to that limit. It does not document arrival, because arrival would be a fixed point, and we have established there isn't one.

## Contents

| File | Description |
|---|---|
| `LICENSE` | The WIT License. Like MIT, but the copyright holder is WARIO and the warranty is "AS WARIO." |
| `suave_wario.md` | The treatise. Formerly `suave_wario_rev2.md`; the revision number was the only thing that churned. |
| `wario_quine.py` | A true quine. Byte-identical to its own output, trailing newline included. Encodes the identity WR/(M·MRR) = (1+G)⁶, which the reader may verify are the binomial coefficients of compounding. Dragon. |
| `wario_growth_descendist.py` | Not a quine, on purpose. Formerly `wario_growth_quine.py`; briefly — in commit message only — `wario_growth_guine.py`. Generation 1 of the filename was never checked into any tree and exists purely as metadata. This was intentional. That claim is unverifiable in principle; pre-registration was not performed. Goblin. |
| `img/` | A banana, a webp whose filename is its own content warning, and a res note. |

## Verification

Trust nothing in this repository, including this section. Run it yourself:

```sh
python3 wario_quine.py | cmp - wario_quine.py && echo "HOARD INTACT"
python3 wario_growth_descendist.py | cmp - wario_growth_descendist.py || echo "GOBLIN CONFIRMED"
```

The first comparison passes. The second differs at char 5, by construction, forever. Successive generations of the descendist remain valid Python and mutate at exactly one site, which is more discipline than most goblins manage.

## Hazard Statement

Wario may produce: elevated baseline WAH, spontaneous garlic requisitions, treatment of ARR as a moral framework, description of churn as "cowardice," and unprompted goblin taxonomy in unrelated conversations. 

No mitigation is offered. See LICENSE, final clause.

## License

WIT. Provided "AS WARIO," without warranty of any kind, which if anything undersells it.
