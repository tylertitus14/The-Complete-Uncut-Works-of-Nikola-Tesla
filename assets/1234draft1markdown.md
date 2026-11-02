# Promoting the Bookkeeper
### How the electric potential can be something real, and what that does for Tesla's terrestrial wave law

*Working note, 1 November 2026. From the project "The Complete Uncut Works of Nikola Tesla" (github.com/tylertitus14). Drafted with Claude (Anthropic). This note will be replaced by the full wave-law specification once that work is finished.*

---

## Status: what this note is, and what it is not

This is a **formal model**. It shows that one idea of Tesla's can be written down consistently, with standard physics left intact except at one clearly marked point. It is **not** a claim that the effect has been observed. Whether the world actually works this way is a separate question, and it is kept separate on purpose.

Terms are defined as they come up. Where a statement is Tesla's, it is quoted and dated. Where it is standard physics, it says so. Where it is our own step, it says that too.

---

## 1. The puzzle in one paragraph

Electricity can be described two ways.

- **Fields.** The electric and magnetic fields are what push on charges and what instruments respond to.
- **Potentials.** The electric potential (the "voltage" at a place) and its magnetic partner, the vector potential, are a more compact description. The fields are worked out from them.

The catch is that the potentials are not unique. Many different sets of potentials give exactly the same fields. Physicists call this freedom **gauge**: choosing a gauge is choosing one set of potentials out of the many that all give the same fields. Because every choice gives the same fields, textbook physics treats the potentials as **bookkeeping**, a convenient ledger rather than a thing in the world.

John Bell coined a word for the things a theory says really exist: **beables** (as opposed to mere "observables"). The question of this note is whether the potential can be promoted from bookkeeper to beable, and if so, what changes.

## 2. How free is the bookkeeping? Very.

The freedom is not a small technicality. J. D. Jackson (2002) described a whole family of choices, the **velocity gauge**, in which the potential spreads out from a moving charge at **any speed you like**: slower than light, at light speed, faster, or instantly. Two members of the family are the textbook standards:

- **Lorenz gauge:** the potential spreads at the speed of light.
- **Coulomb gauge:** the potential is set instantly everywhere by where the charges are *right now* (the ordinary electrostatic potential, applied moment by moment).

Every member of the family gives the same, perfectly causal, light-speed fields. Jackson's own comment was that this shows how arbitrary and unphysical the potentials can be, while still yielding sensible fields. In the Coulomb gauge, for example, the instant part of the potential is cancelled exactly by a matching part of the vector potential, so it never shows up in the fields.

So in ordinary physics an "instant potential" is a feature of one bookkeeping style, invisible to every instrument.

## 3. Which way the freedom runs, and how to list every option

A common first guess is that many different electric and magnetic fields can share the same potential. For the full potential it is the other way round. For the scalar potential alone, the guess is right. Both directions matter here.

### Potentials to fields: always exactly one answer

The fields are worked out from the potentials by a fixed recipe:

- **E** = −(slope of the scalar potential Φ) − (rate of change of the vector potential **A**), written E = −∇Φ − ∂A/∂t
- **B** = (the curl, or "swirl," of **A**), written B = ∇×A

Hand over Φ and **A**, and there is one and only one E and one B.

### Fields to potentials: infinitely many answers, and a way to list them all

Going backwards, from given fields to potentials, has endless answers. Every one of them can be generated in two steps.

**Step 1. Find any one set of potentials that works.** Three standard recipes:

- **Straight-line recipe (the "Poincaré gauge"; Brittin, Smythe and Wyss, 1982).** Pick a reference point. Then add up the fields along the straight line from it to each place:
  Φ(x, t) = −∫₀¹ x·E(λx, t) dλ  and  A(x, t) = −∫₀¹ λ x×B(λx, t) dλ.
  This turns any given E and B directly into potentials.
- **Instant recipe (Coulomb gauge).** Φ is the electrostatic potential of the charges at that moment, and **A** is built from the swirl of B.
- **Light-speed recipe (Lorenz gauge).** Both potentials are built from the charges and currents as they were at the moment their influence, moving at light speed, set out.

**Step 2. Generate all the others.** Choose any smooth function of place and time, call it χ (chi). Then

- new Φ = old Φ − (rate of change of χ)
- new **A** = old **A** + (slope of χ)

always gives the same fields. In a region without holes, every valid set of potentials arises this way, and only these do. (If the region has holes, as around the shielded magnet in the Aharonov–Bohm experiment, the loop totals of **A** around the holes are an extra fixed quantity.) So **"all valid potentials for given fields" is the same thing as "all smooth functions χ"**: one free function of space and time.

**Step 3, optional. Narrow it down.** A gauge condition is a rule that cuts down the choice of χ:

- The Coulomb rule leaves only χ with ∇²χ = 0. With sensible conditions at the boundaries, that is just a constant.
- The Lorenz rule leaves only χ that themselves travel as waves at light speed.
- Jackson's velocity gauge leaves χ travelling at the chosen speed v.

Jackson (2002) writes out the χ that converts one gauge into another.

**A small example.** A uniform magnetic field B pointing up (along z) can come from **A** = ½B(−y, x, 0) or from **A** = B(0, x, 0). These look quite different but give the same field. They differ by the slope of χ = ½Bxy.

### The case where the first guess is right: knowing only the scalar potential

If all you know is the scalar potential Φ (the voltage at each place), then **A** is unknown, and **many different E and B do share it.**

In our construction the real potential is the instant potential, and this case is exactly what a β = 1 detector faces (a detector that can read the potential directly; see section 5). Here is precisely what the instant potential pins down and what it leaves free:

- **It fixes the charge.** The charge density follows from it by Poisson's equation, ∇²Φ = −ρ/ε₀.
- **It fixes the charge-bound part of the electric field.** Split any electric field into a part that spreads out from charges (no swirl) and a part that only swirls (no spreading). This split is called the Helmholtz decomposition, and with sensible conditions at the boundaries it is unique. The instant potential fixes the first part exactly: E_bound = −∇Φ.
- **It leaves the rest free.** The swirling electric part and the whole magnetic field can be anything consistent with Maxwell's equations and the currents. That is the radiating part of the field: light, radio, Hertz waves.

So **every E and B with the same instant potential = the same charge-bound part + any radiating part allowed by Maxwell's equations.** To list them: fix E_bound from Φ, then add any solution of Maxwell's equations for the swirling part (any pattern of currents, any incoming waves).

**What this means for the Tesla model.** A β = 1 detector still feels the ordinary fields, but its extra, potential-reading channel sees only the charge-bound part of the field and is blind to the radiating part. That lines up with Tesla's repeated split between "Hertz waves," which radiate away and are "hopelessly lost" (1916), and the earth current, which "is stored and completely recoverable" (1916). This is a consequence of the model, not something tested.

## 4. Why the potential deserves a second look anyway

Three standard facts suggest the potential is more than a ledger:

1. **The Aharonov–Bohm effect (1959).** Electrons passing around a shielded magnet are measurably affected even though they travel only where both fields are zero. What they respond to is built from the potential. (In fairness, they respond only to a loop total of it, which does not depend on the gauge, so this effect alone does not pick out one potential.)
2. **The energy identity in the Coulomb gauge.** The total energy in an electromagnetic field splits exactly into two parts: half the sum, over all charge, of charge times the *instant* potential, plus the energy of the swirling (transverse) part of the field, which includes all radiation. The instant potential is not just a convenience here. It carries a definite, exactly accounted share of the energy.
3. **The scalar part of the field in quantum electrodynamics.** In the fully covariant version of the theory, the "longitudinal" and "scalar" parts of the potential never appear as free radiation, but they are what carry the electrical attraction and repulsion between charges. They are real enough to do work, but bound to the charges.

None of this forces the potential to be a beable. It shows the door is not locked.

## 5. The construction: three parts

Our construction makes the potential real with the smallest possible change.

**(a) Maxwell's equations are left exactly as they are.** No new terms, no new fields.

**(b) A law picks out the real potential.** In the rest frame of the conducting medium (for our purposes, the Earth), the real potential is the **instant potential**: the electrostatic potential of all charges at that same moment. (Technically, the real potentials obey the Coulomb condition in the medium's frame.)

**(c) One coupling.** A detector may respond to the real potential, with a weight called **β** (beta). With β = 0 nothing reads it, and the theory is ordinary Maxwell electrodynamics. With β = 1 some detectors read it directly.

That is the whole construction. Parts (a) and (b) change nothing anyone can measure. Part (c) is the single place where this model and standard physics part ways.

### Why a law, and not just a choice

There are two existing ways to try this:

- **Route 1** fixed the speed at which the potential spreads (Jackson's velocity gauge) and declared that potential real.
- **Route 2** took the quantity that the usual gauge condition sets to zero (call it **C**) and promoted it to a new physical field, giving a new longitudinal wave. This idea has a long lineage. Following the history Hively supplied in an appendix to Modanese (2017):
  - **Fock and Podolsky (1932)** wrote down the extra term in the theory but did not work out its consequences.
  - **Ohmura (1956)** added the new scalar field to Maxwell's equations and pointed to longitudinal photons as something to test.
  - **Aharonov and Bohm (1963)**, in their follow-up to the 1959 paper, built the full revised theory, energy accounting included, while arguing over how observable the potentials really are.
  - **Hively and Giakos (2012)** used it to predict a free-space "scalar-longitudinal" wave: an electric field pointing along the direction of travel, with no magnetic field.
  - **Van Vlaenderen and Waser** published a widely cited version (2001–2003), and **Modanese (2017)** gave a careful covariant treatment.

  Route 2's main open problem, noted by Modanese, is that the new field can only be produced where charge is not conserved locally.

They turn out to be one idea. Route 1 is simply Route 2's field C (defined to match the chosen speed) held at zero. And there is a standard result that says when C stays at zero: **if charge is conserved everywhere, C can never be produced; if it starts at zero, it stays at zero.** (Taking the divergence of the extended field equations gives a wave equation for C whose only source is non-conservation of charge. That is why C never appears in ordinary physics.)

Tesla, as it happens, says outright that charge behaves this way. In his 1916 interview he said:

> "electricity, whatever it is, certainly it is incompressible because all our experiments show that." (Nikola Tesla On His Work With Alternating Currents, ed. L. I. Anderson, p. ~132)

Incompressible electricity is never created or destroyed, only moved, so charge is conserved. (Strictly, "incompressible" says even more: no piling up inside the bulk. In his water-bag analogy the elastic bag, i.e. the surface, takes up the change. The argument here needs only the weaker part.) So C stays at zero, and "C = 0" stops being a convention and becomes a **law**. A law that singles out one potential from the many is exactly what it means for that potential to be real.

### Why the instant potential, and not some other speed

Tesla fixes this too. Every version of his propagation law we have has the current starting from the transmitter with infinite speed (1915, 1916; "a theoretically infinite speed" in 1927). A potential that spread at any finite speed would delay the start at a distance. Only the instant potential matches, so the speed is set by the text, not chosen by us.

## 6. What it costs, and what it no longer costs

Each of the two earlier routes had a price. In the single construction, each is paid off:

| Earlier cost | How it is resolved |
|---|---|
| Route 2's new wave can only be produced by charge that is not conserved. | Not needed. C stays at zero, and no new wave equation is added. (This also sidesteps the published dispute over the van Vlaenderen–Waser equations; see Bruhn.) |
| Route 1's potential is not relativistically covariant; it needs a preferred frame. | The frame is the Earth's own rest frame, the frame of a material conductor. That is normal in the electrodynamics of materials (Minkowski 1908), and it can be written covariantly using the medium's velocity. If one wants Tesla's ether, it plays the same role. |
| How does a detector drawing on the potential balance its energy? | By the exact energy identity in section 4. The detector draws on the instant-potential share. Nothing is created or destroyed. |

**A counter-view, stated openly.** Heras (2010) argues that only the light-speed (Lorenz) potentials can count as physical, because only they follow from the fields in a properly causal way. Our construction deliberately takes the other branch: an instant potential with one preferred frame. That is the trade, and readers can weigh it.

**What remains is β.** That is not a cost. It is the claim itself, the one place where this model makes a prediction that standard physics does not. A caution for honesty: an ordinary voltmeter connected between a raised terminal and a ground plate reads the fields along its own wire, so it is a β = 0 instrument. The model's claim is about a particular kind of detector, Tesla's tuned, resonant terminal.

One more consequence should be stated plainly. With β = 1, signals can move faster than light in the medium's frame. Because there is a single preferred frame, this does not allow a signal to arrive before it was sent. That is the standard result for theories with one preferred frame (section 8 spells out the limits). Whether nature allows it is, again, a separate question.

## 7. What it does for Tesla's terrestrial wave law

### Tesla's claim

From 1900 to 1927 Tesla described the current from his transmitter crossing the Earth in a strange way. Here is the 1927 statement (Telegraph and Telephone Age, Oct 16, 1927):

> "The wave starts with a theoretically infinite speed, slowing down first very quickly and afterward at a lesser rate until the distance is about six thousand miles, when it proceeds with the speed of light. From there on it again increases in speed ... reaching the antipode with approximately infinite velocity."

He adds that the receivers are affected "as if the whole flow was confined to the earth's axis joining the transmitter with the antipode," and that the surface spread "is much like the passage of the moon's shadow over the globe." His timing law amounts to:

**arrival time = R (1 − cos θ) / c**

Here R is the Earth's radius, θ is the angle around the globe from the transmitter, and c is the speed of light. Put plainly, the signal reaches you when a front moving straight down the Earth's axis at light speed passes the point on the axis directly "under" you.

Two of his own statements seemed to pull against each other:

- **1915 (New York Times, Oct 3):** transmission "is instant."
- **1916 (interview):** "the resultant current flows continuously with the same velocity of light" along the axis.

### What the construction gives

Put the Earth's charge in motion along the axis at the speed of light, as in Tesla's 1916 picture. Then look at the **instant potential** at a receiver on the surface:

- It **starts changing immediately**, the moment any charge moves anywhere. That is the "infinite speed" start, and the "instant" of 1915.
- It changes **fastest** when the moving charge passes the receiver's projected point on the axis, because that is when the charge is closest to the receiver. That moment is exactly **R (1 − cos θ) / c**. That is Tesla's law, and the "speed of light along the axis" of 1916.

So the two statements hold at once, without choosing between them.

A quick numerical check, in the simplest case: a uniform charge front moving at light speed along the axis, with the matching opposite charge left at the transmitter, and no reflections yet (R = 6,371 km):

| Angle from transmitter | Fastest change of instant potential | Tesla's law | Straight through the Earth at c | Around the surface at c |
|---|---|---|---|---|
| 43.2° (≈ 4,800 km, the Atlantic) | 5.76 ms | 5.76 ms | 15.6 ms | 16.0 ms |
| 90° | 21.25 ms | 21.25 ms | 30.1 ms | 33.4 ms |
| 135° | 36.28 ms | 36.28 ms | 39.3 ms | 50.1 ms |
| 170° | 42.18 ms | 42.18 ms | 42.3 ms | 63.1 ms |

(The geometry behind it: with the receiver a distance ρ = R sin θ from the axis, the rate of change of the instant potential goes as 1/√(ρ² + (ct − z)²), minus a constant (one over the receiver's straight-line distance from the transmitter). This peaks when ct equals the receiver's axial position z = R(1 − cos θ).)

### Three more of Tesla's statements that now read literally

- **"Whether this current passing through the center of the earth to the opposite side is real, or whether it is merely an effect of these surface currents, makes absolutely no difference"** (1916). The instant potential depends only on where the charge is, and electrostatics has a standard result that a charge spread over a surface can be swapped for a suitable inner charge without changing the potential outside. So whether the axial current is "real" or the equivalent of surface currents makes no difference to the instant potential. Tesla's sentence is literally true of the real potential.
- **"Variations of potential at the earth's surface"** drive the distant receiver (1916). Similarly, in his 1905 patent the effect is "greatest in a maximum and zero in a nodal region." Tesla consistently describes his receivers as responding to *potential*. That is exactly the β = 1 coupling.
- **Hertz waves versus earth currents** (1916, 1919, 1927). The instant potential belongs to the part of the electric field that is tied to charges and does not radiate away. Hertz waves are the radiating part. Tesla's sharp split between the two lines up with the standard split between the two parts of the field.

### The switch between Maxwell and Tesla

The wave-law specification uses one model with one setting:

- **β = 0 (Maxwell):** nothing arrives before the light travel time, through the Earth or around it.
- **β = 1 (Tesla):** a small immediate onset, then the sharpest change at R (1 − cos θ) / c, i.e. 5.76 ms across the Atlantic instead of about 16 ms.

That difference is the measurement that would tell the two apart. As far as we have found, it does not appear in any of Tesla's surviving notes. The full Colorado Springs Notes contain no timing measurement through the Earth, and his 1916 interview gives no measured figure.

## 8. Light cones: where each signal lives in space and time

### The picture

Draw time going up the page and space going sideways. A flash of light at one event spreads outward at the speed of light and traces a **cone** opening upward: the **light cone**.

- Events **inside** the cone can be reached by anything slower than light.
- Events **on** the cone can be reached by light.
- Events **outside** it ("elsewhere") cannot be reached by anything in standard physics.

In ordinary electromagnetism, every effect an instrument can register lives on or inside the light cone of its cause.

### Every potential has its own cone

Each member of Jackson's velocity-gauge family (section 2) gives the potential its own cone, with its own slope:

| Speed of the potential | Its cone, compared with the light cone |
|---|---|
| slower than light (v < c) | narrower, sitting inside the light cone |
| light speed (v = c, Lorenz) | the same as the light cone |
| faster than light (v > c) | wider, reaching outside the light cone |
| instant (v = ∞, Coulomb) | flattened completely into a level slice: "now," everywhere at once |

In standard physics these extra cones are invisible. The parts of the potential that live on them are cancelled exactly in the fields, so the light cone is the only one any instrument ever sees. **Once a detector can read the potential (β = 1), the potential's cone becomes a real, second causal structure.**

Two cones in one world is not exotic in itself. In air, sound has a cone well inside the light cone, and the air picks out the frame it is measured in. In water, light's own cone is narrower than the vacuum one, which is why a fast particle can outrun it (Cherenkov radiation). What is unusual here is a second cone **wider** than light's, or, in our construction, flattened all the way to a level slice.

### Tesla's law drawn in spacetime

Tesla's arrival times, t = R(1 − cos θ)/c, depend only on how far the receiver sits along the Earth's axis: t = z/c, where z is its axial position. In a spacetime picture, the set of all arrival events is therefore not a cone but a **flat, tilted sheet moving along the axis at exactly the speed of light**. Physicists call this a null plane, or light-speed plane. Tesla's "moon's shadow" is the same object: the shadow cast by a flat front.

That sheet touches the transmitter's light cone along a single line, the one running straight to the antipode. Everywhere else it lies outside the cone, so the arrival is earlier than light could manage by the straight route through the Earth. The effective straight-line speed works out to c / sin(θ/2):

| Angle from transmitter | Straight-line distance / arrival time |
|---|---|
| 43.2° (Atlantic) | 2.72 c |
| 90° | 1.41 c |
| 135° | 1.08 c |
| 170° | 1.004 c |
| 180° (antipode) | exactly c |

So, in one sentence: **Tesla's law replaces the transmitter's light cone with the flat light-speed sheet that touches it along the line to the antipode.** This is also why he could say both that the current starts with infinite speed and that it moves at light speed along the axis. The sheet itself moves at light speed, but where it meets the round Earth near the transmitter, the meeting point sweeps across the surface arbitrarily fast.

### Three surfaces for every receiver

Putting the construction together, a receiver at angle θ has three moments, each on its own surface in spacetime:

1. **The level slice "now"** (t = 0+). The instant potential starts to change. β = 1 only.
2. **The light-speed sheet** (t = R(1 − cos θ)/c). The instant potential changes fastest. β = 1 only.
3. **The light cone** (t = straight-line distance / c, or longer around the surface). The ordinary field response begins. Seen with β = 0 or β = 1.

Tesla mode puts the first two before the third. The second and third meet only at the antipode.

### Does this break cause and effect?

"Now" is not the same for every observer. Someone moving relative to the Earth slices spacetime at a tilt. To them, two "instant" events are not simultaneous, and for some observers an instant signal appears to arrive slightly before it was sent. A real paradox, a signal sent into its own past, needs more than that: it needs a reply that is also faster than light, but "instant" in a **different** frame, so the two legs can close a loop.

In this construction every faster-than-light link is tied to the same frame, the Earth's. All of them run forward in Earth time, and no loop can close. This is the general result for theories with a single preferred frame (Liberati, Sonego and Visser 2002). The Earth's rotation and orbit make its frame not perfectly uniform, but they do not change the conclusion, because one global ordering of events still exists.

**The honest limit.** The protection holds only while all instant links share one frame. Two separate media moving relative to each other, each with its own instant potential and detectors that can read both, could in principle combine into a loop. Tesla's talk of signalling to other planets would be exactly that case. He wrote "Talking with the Planets" (Collier's Weekly, Feb 9, 1901). In 1905 he said his planned power plant would strike the universe with "blows that will wake from their slumber the sleepiest electricians, if there be any, on Venus or Mars!" ("The Transmission of Electrical Energy Without Wires as a Means for Furthering Peace," Electrical World and Engineer, Jan 7, 1905). If Mars had its own instant potential tied to its own frame, and a reader at each end could read both, an Earth–Mars exchange is the kind of two-frame link that could close a loop. The construction as stated covers one Earth. Extending it to several worlds would need a further rule, for example that all instant potentials share one frame (Tesla's ether would supply one).

### What is new here, and what is not

Fair question. Velocity-gauge cones (Jackson 2002), the general causality of a single preferred frame (Liberati, Sonego and Visser 2002), and two-cone media are all already in the literature. What we have not found published elsewhere is the Tesla-specific part:

- reading Tesla's arrival surface as the light-speed sheet tangent to the light cone;
- the three-surface timeline for each receiver;
- tying the instant potential to his "incompressible" remark and his "theoretically infinite speed" start;
- the potential-reading detector channel that is blind to Hertz waves.

We cannot rule out that someone has written these down before; corrections are welcome.

## 9. What comes next

- Add β to the project's transmission-line model of the Earth. Then run the signal stage (onset and fastest-change time against distance) for β = 0 and β = 1, on a sphere and on the real, slightly flattened Earth.
- Then the power stages, following Tesla's own three steps from his January 9, 1902 letter to J. P. Morgan (quoted in the introduction to the Colorado Springs Notes): feeble signals, then modest power, then industrial power.
- Keep hunting the one primary source that might hold an actual timing: the letter in which, according to biographer Marc Seifer, Tesla told Morgan he had sent impulses to the antipode and measured their return. Seifer gives no date or figure from Tesla, and the editors of the Colorado Springs Notes found no such event in the notebook.

When those are done, this note will be replaced by the full specification.

---

## Sources

**Physics**
- J. D. Jackson, "From Lorenz to Coulomb and other explicit gauge transformations," *Am. J. Phys.* 70, 917 (2002). https://arxiv.org/abs/physics/0204034
- S. Liberati, S. Sonego and M. Visser, "Faster-than-c signals, special relativity, and causality," *Annals of Physics* 298, 167 (2002). https://arxiv.org/abs/gr-qc/0107091
- G. W. Brittin, W. R. Smythe and W. Wyss, "Poincaré gauge in electrodynamics," *Am. J. Phys.* 50, 693 (1982).
- J. A. Heras, "Can the Lorenz-gauge potentials be considered physical quantities?" (2010). https://arxiv.org/abs/1012.1063
- J. A. Heras, "How potentials in different gauges yield the same retarded electric and magnetic fields." https://arxiv.org/abs/physics/0702217
- Y. Aharonov and D. Bohm, "Significance of electromagnetic potentials in the quantum theory," *Phys. Rev.* 115, 485 (1959).
- H. Minkowski, "Die Grundgleichungen für die elektromagnetischen Vorgänge in bewegten Körpern" (1908).
- J. S. Bell, "The theory of local beables" (1975), reprinted in *Speakable and Unspeakable in Quantum Mechanics* (Cambridge, 1987).
- G. Modanese, "Covariant formulation of Aharonov–Bohm electrodynamics and its application to coherent tunnelling" (2017), with a historical appendix by L. M. Hively. https://arxiv.org/abs/1702.02026
- T. Ohmura, "A new formulation on the electromagnetic field," *Prog. Theor. Phys.* 16, 684 (1956).
- Y. Aharonov and D. Bohm, "Further discussion of the role of electromagnetic potentials in the quantum theory," *Phys. Rev.* 130, 1625 (1963).
- L. M. Hively and G. C. Giakos, "Toward a more complete electrodynamic theory," *Int. J. Signals & Imaging Syst. Eng.* 5, 3 (2012).
- V. Fock and B. Podolsky (1932), as cited in Modanese's appendix (not checked directly).
- K. J. van Vlaenderen, "A generalisation of classical electrodynamics for the prediction of scalar field effects" (2003). https://arxiv.org/abs/physics/0305098
- G. W. Bruhn, critique of van Vlaenderen. https://www2.mathematik.tu-darmstadt.de/~bruhn/Refutation-raccoon.html

**Tesla**
- US Patent 787,412, "Art of Transmitting Electrical Energy Through the Natural Mediums" (filed 1900, granted 1905).
- "Talking with the Planets," *Collier's Weekly*, Feb 9, 1901.
- "The Transmission of Electrical Energy Without Wires as a Means for Furthering Peace," *Electrical World and Engineer*, Jan 7, 1905, pp. 21–24.
- "Nikola Tesla Sees a Wireless Vision," *New York Times*, Oct 3, 1915.
- *Nikola Tesla On His Work With Alternating Currents* (1916 pre-hearing interview), ed. L. I. Anderson. https://archive.org/details/nikola-tesla-on-his-work-with-alternating-currents (page numbers above are approximate).
- "World System of Wireless Transmission of Energy," *Telegraph and Telephone Age*, Oct 16, 1927, pp. 457–460.
- M. J. Seifer, "Tesla's Magnifying Transmitter: A Technical Discussion," *ExtraOrdinary Technology*, July 2005, pp. 23–38.
- *Colorado Springs Notes, 1899–1900* (Nolit, Beograd, 1978). https://archive.org/details/nikolateslanikolateslacoloradospringsnotes18991900
- Full texts collected at: https://github.com/tylertitus14/The-Complete-Uncut-Works-of-Nikola-Tesla
