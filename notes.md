# General gauge theory
[HAMILTON 2015]

All the fundamental forces arise from constraints imposed by local gauge symmetries.

gauge group = G
particles ≅ irreps of G
gauge field ≅ coefficients of connection on principle G-bundle over spacetime
gauge bosons ≅ quanta of gauge field (Spin-1 particles, represented as 1-forms)

In gauge theory, we have an action of G on
	𝒞 = matter fields ⊕ gauge fields = C∞(M → V) ⊕ ∧¹(M, 𝔤)
given by
	g·(Ψ ⊕ A̲) = g·Ψ ⊕ (gA̲g' - (dg)g')
Given Eqns of Motion (e.g., via a Lagrangian), the space of solutions 𝒮 ⊂ 𝒞 is invariant under G.

Global GTs affect local and ∂-derivative quantities identically. (Since ∂g = 0)
Local GTs affect local and ∂-derivative quantities differently.
If f: M → Aut(V) is a local gauge transformation, then an Ehresmann connection ∂ ↦ ∇(x) = ∂ + A(x) may be introduced to "undo" the affect of f(x) on derivative quantities. The gauge field, A(x), depends on f(x).
	d ↦ d^A = d + A "exterior covariant derivative"

This is the sense in which a gauge theory "extends" a global symmetry to a local symmetry.
General relativity is the what you get when you localise global translation symmetry to local diffeomorphism invariance.

gauge field strength ≅ curvature of connection

field strength: F = d^A A
Bianchi identity: d^A F = 0 [Hamilton, Theorem 5.14.2]


TERMS IN A LAGRANGIAN MUST NOT BE OF ORDER > 4 LESS THE THEORY BE UNRENORMALISABLE.

"The Lagrangians that are important in physics are mainly restricted by
three principles:" [Hamilton §7]

The Lagrangian should be:
- Symmetric
	Gauge invariant and Lorentz invariant
- Renormalisable

- Free of gauge anomalies
	It is possible for symmetries of classical field theories are broken when quantised. Such a symmetry is called anomalous.


## Yang–Mills theory

... is the theory of gauge bosons only, without the matter fields.
ℒ_YM determines the dynamics for the gauge field.

A connection ∇ = ∂ + A involves a 𝔤-valued 1-form A, transforming as A ↦ gAg' + (∂g)g'.
The curvature F = dA + A∧A of A is a 𝔤-valued 2-form, transforming as F ↦ gFg'

Upon *choosing* a Ad-invariant positive-definite scalar product ⟨ , ⟩ on 𝔤, the Yang–Mills Lagrangian is
ℒ_YM = -1/4 ⟨F^μν, F_μν⟩ = -1/4 F^iμν F_iμν
where Latin indices ij... denote components of F_μν ∈ 𝔤 with respect to an ⟨ , ⟩-orthonormal basis.
(Existence of such an scalar product is guaranteed by the compactness/semi-simplicity of the gauge group G.)
The *only* Lorentz and gauge invariant free field Lagrangians for A which are at most quadratic in A and involve derivatives of order <= 1 are constant multiples of ⟨F, F⟩ (Lorentz invariant) or ⟨F, ★F⟩ (restricted Lorentz invariant) [FOLLAND pg. 293].

Any compact simple Lie group G is of the form
	G = G₁⊕⋯⊕Gₛ
where each Gᵢ is a compact simple Lie group or U(1).
The Ad-invariant positive-definite scalar products ⟨ , ⟩ of 𝔤 are determined by positive constants for each Gᵢ.
These s constants are called *coupling constants*.

Thus, the Yang–Mills Lagrangian involves the choice of coupling constants.

nonabelian[G] ⟹ nonlinear terms from ℒ_YM ⟹ interactions between gauge bosons




# Standard model

Gauge group G = (U(1)⊕SU(2)⊕SU(3))/ℤ₆.

Complete fermionic content is described by an associated vector bundle of rank 90.
90 = 3 generations of (2 particle/antiparticle pairs of (8 left-handed + 7 right-handed)) fermions

fermions = [(generation, anti, handedness, i)
	for generation ∈ 1:3,
		anti ∈ (false, true),
		handedness ∈ (:left, :right),
		i ∈ handedness == :left ? 8 : 7]

Reasons to Suspect the Standard Model is Incomplete
[HABER 1985]

1) it contains many arbitrary assumptions and parameters
2) QED is not asymptotically free, suggesting it is the EFT of a more fundamental theory.


## Discrete Symmetries

C: charge conjugation
P: parity
T: time reversal

**CPT Theorem**
If a QFT is
- Lorentz invariant
- local
- unitary (Hermitian Hamiltonian)
then it must admot CPT symmetry.

If |c,p,t⟩ represents the universe, and
	C|c,p,t⟩ = |-c,p,t⟩
	P|c,p,t⟩ = |c,-p,t⟩
	T|c,p,t⟩ = |c,p,-t⟩
represents the discrete transformations, we have
	CPT|c,p,t⟩ = |-c,-p,-t⟩ ≅ |c,p,t⟩
by CPT symmetry.

In particular, we have CP ≅ T, since
	CP|c,p,t⟩ = |-c,-p,t⟩ ≅ |c,p,-t⟩ = Z|c,p,t⟩
and similarly PT ≅ C and TC ≅ P.

2002: Oscar Greenberg: proof that CPT violation ⇒ broken Lorentz symmetry

Parity is maximally broken by weak interactions.


# Strong CP Problem

QCD is very successful.
The most general properties allowed by colour gauge symmetry in the context of SR and QM are almost perfectly what we observe about quarks and gluons.

However, QCD permits CP violation, but this has not been observed.
QCD fails to forbid CP violation.
This is the _strong CP problem_, one of the major unsolved problems in (particle) physics. "A serious flaw of the standard model." [Dan-di Wu 1991]

In QCD, a total divergence term in Lagrangian
	ℒ ∝ ⟨F, ★F⟩
the θ term, allows CP violation.
∫ ⟨F, ★F⟩ Ω ∝ ∫ ∂¹(A²∂³A⁴ϵ¹²³⁴) Ω = ∫ d(A²∂³A⁴ϵ¹²³⁴★dx¹) = ∮ A²∂³A⁴ϵ¹²³⁴★dx¹
So the associated current is V¹ = ϵ¹²³⁴A²∂³A⁴.

CP violation gives rise to a nonzero neutron dipole moment.
Measurement of neutron dipole moment: d_n = (0.0 ± 1.1)×10^-26 e·cm ≈ 0
This implies the restriction |θ| < 10^-9.

The strong CP problem is a fine-tuning problem: why is θ so small?


## Solutions to the Strong CP problem

[Agrawal 2018]
Roughly two categories:
	1) Nelson–Barr
		impose discrete symmetries like CP or P that enforce θ = 0
	2) Peccei–Quinn
		invokes global U(1) symmetry
		1.1) massless (up-)quark solution -> θ becomes unphysical
			however, lattice QCD calculations show that all quarks are massive
		1.2) QCD axion


## Axions - Peccei--Quinn theory

Axions are a dark matter candidate.

Conclusions of [PECCEI 2006]:
"In my view, after more than 25 years, the preferred solution to the strong CP problem remains still the idea that the Standard Model has an additional U(1) symmetry. Such a solution, necessarily, predicts the existence of a concomitant axion."



# Asymptotic Freedom
[WILCZEK 2005]

_Asymptotic freedom_ refers to the decrease in strength of interactions at short distances, as in QCD.

_Screening_ is the tendency for a bare charge to conjure a cloud of virtual particles around it which decrease the effective charge of the original charge.
This is a problem in QED, because screening should continue so long as there is uncancelled charge---that is, until the charged particle is completely covered in a virtual cloud resulting in zero effective charge.
Yet, we observe bare charges.

_Antiscreening_ is the tendency for a bare charge to conjure a cloud of virtual particles around it which enhance the charge.
This is a runaway process: a single charge will thrust into being a virtual cloud which results in an even greater charge, attracting more virtual particles, and so on.
Antiscreening is exhibited in QCD.
This explains quark confinement: quarks cannot exist in isolation or in groups of nonzero total colour charge, because their energy would be unbounded by antiscreening.
Instead, quarks can exist in quark-antiquark pairs (or any colourless hadron) because the virtual cloud and anticloud cancel their colour charges.
Quarks and antiquarks bound together (a.k.a., mesons) can be accommodated with finite energy, though either quark in isolation would cause an infinite disturbance.

Antiscreening results in asymptotic freedom.

The theories which exhibit asymptotic freedom are the nonabelian gauge theories, a.k.a., Yang--Mills theories.

QED			nonabelian QCD
screening	antiscreening
charge		colour(s)
photon		gluon(s)
Force carrier charge:
uncharged	charged

It is the fact that gluons are themselves (colour-)charged which is responsible for antiscreening, which does not occur in QED.


