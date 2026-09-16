# From a decimal hint to a faithful quotient

## A mathematical case study in observation, correction, and reflection

16 September 2026

**Evidence label:** ordinary mathematical proofs with explicit domains; no proof-assistant check or historical-priority claim. This is a contemporary case study of a research method, not a claim about Euler's historical discoveries. It contains no private project source, internal archive, or blind-evaluation material.

The starting observation is the Fibonacci-weighted expansion of 1/89. The durable result is not that addition and multiplication are secretly identical. It is a precise answer to when a quotient that normally loses information becomes faithful on a certified source domain.

## 1. Observe, then state the object correctly

Let \(F_0=0,F_1=1,F_{n+2}=F_{n+1}+F_n\). Multiplying the formal series by its recurrence polynomial gives

\[
\sum_{n\ge0}F_nz^n=\frac{z}{1-z-z^2}.
\]

The real series converges at \(z=1/b\) for every integer \(b\ge2\), because Fibonacci growth is bounded by a constant times \(((1+\sqrt5)/2)^n\). Thus

\[
\boxed{\frac1{b^2-b-1}=\sum_{n\ge1}\frac{F_n}{b^{n+1}}.}
\]

At base 10 this gives 1/89. It is not a literal concatenation of Fibonacci numbers in decimal digits: carries change the visible digits. A successful observation begins by naming the weighted series rather than a stronger false pattern.

## 2. Make the analogy an algebra

Put

\[
A=\mathbb Z[t]/(t^2-t-1).
\]

Every element has a unique form \(u+vt\), and

\[
t^n=F_nt+F_{n-1}\quad(n\ge1).
\]

Induction proves the formula using \(t^2=t+1\). Multiplication by \(t\), in the basis \(1,t\), is the additive state update

\[
C=\begin{pmatrix}0&1\\1&1\end{pmatrix}.
\]

The inverse difference between integer scaling and this recurrence transport is

\[
(bI-C)^{-1}=\frac1{b^2-b-1}
\begin{pmatrix}b-1&1\\1&b\end{pmatrix}.
\]

Expanding the inverse as \(\sum_{n\ge0}C^n/b^{n+1}\) recovers the weighted series. Consequently 89 is the determinant and lattice index of the defect \(10I-C\), not an unexplained decimal coincidence.

## 3. Try to break the proposed equivalence

For \(M=b^2-b-1\), evaluation gives

\[
E_b(u,v)=u+bv\pmod M.
\]

It intertwines recurrence multiplication with multiplication by \(b\), but it is not an invertible change of basis. The nonzero vector \((-b,1)\) is invisible. In particular, \(\{1,10\}\) is not a two-dimensional basis of \(\mathbb F_{89}\).

This distinction has an observable consequence. Modulo 5 at base 3, scalar multiplication by 3 has order 4. But direct recurrence algebra gives \(C=3I+N\), \(N\ne0\), \(N^2=0\) over \(\mathbb F_5\). Its nontrivial unipotent factor has order 5, so \(C\) has order 20. Scalar periodicity has erased part of the state.

The failed stronger statement is useful: it identifies the kernel as the object to study next.

## 4. The exact kernel test

For a homomorphism \(E:\mathbb Z^d\to G\) and source set \(S\),

\[
\boxed{E|_S\text{ injective}\iff(S-S)\cap\ker E=\{0\}.}
\]

**Proof.** \(E(x)=E(y)\) iff \(x-y\in\ker E\). ∎

For the integer box \(B_H=[-H,H]^d\cap\mathbb Z^d\), the difference set is exactly \(B_{2H}\). The smallest invisible displacement therefore determines the sharp recoverable height.

### Sharp Fibonacci theorem

For \(b\ge3\),

\[
\boxed{E_b\text{ injective on }[-H,H]^2\cap\mathbb Z^2
\iff 2H<b-1.}
\]

**Proof.** A collision gives a nonzero \((u,v)\) with \(|u|,|v|\le2H\) and \(M\mid u+bv\). If \(|u|,|v|\le b-2\), then

\[
|u+bv|\le(b+1)(b-2)=M-1.
\]

Divisibility forces \(u+bv=0\), and \(|u|<b\) then forces \(u=v=0\). Conversely, \((-1,b-1)\) is a kernel vector of max-norm \(b-1\). It is a difference of two box points as soon as \(2H\ge b-1\). ∎

At base 10, all 81 points of \([-4,4]^2\) are distinguished. At height 5, `(0,-4)` and `(-1,5)` collide because their evaluations differ by 89.

The quotient is globally lossy but provably faithful for a bounded task. That is a stronger and more useful conclusion than either “the map is an equivalence” or “the map loses information, so it is useless.”

## 5. A general constructive theorem

Let \(P=X^d+\sum_{i<d}p_iX^i\) be monic, \(H_P=\max|p_i|\), and source coefficients obey \(|u_i|\le H\). If

\[
b\ge\max(2,H_P+2H+1),
\]

then evaluation modulo \(P(b)\) is injective on those normal forms and has an explicit decoder.

**Proof.** Put \(S_b=1+b+\cdots+b^{d-1}\). The base bound gives \((H_P+2H)S_b\le b^d-1\), hence \(P(b)\ge2HS_b+1\). Every allowed evaluation has absolute value at most \(HS_b<P(b)/2\), so its centered residue is the actual integer evaluation. Recover coefficients successively as balanced base-\(b\) digits. Since \(b>2H\), each allowed digit is unique. Reject an oversized digit or a nonzero remaining high quotient. ∎

The source-height premise is indispensable. A successful decoder may find a small representative of an observation produced by a larger, unallowed source. Decoding cannot certify the premise on which its validity depends.

For circuit composition, reduce \(t^{i+j}=\sum_kT_{kij}t^k\). If inputs have coordinate bounds \(U_i,V_j\), the product has bounds

\[
W_k=\sum_{i,j}|T_{kij}|U_iV_j.
\]

This is the triangle inequality applied to the coefficient expansion. Every multiplication must refresh the bound; the coefficient box is not a subring. No efficiency advantage follows automatically.

## 6. Two insufficient views can be sufficient together

On \([-5,5]^2\), neither \(E_{10}\) modulo 89 nor \(E_{11}\) modulo 109 is injective. Nevertheless their pair is injective.

**Proof.** A joint collision gives \(|u|,|v|\le10\) and

\[
u+10v=89m,\qquad u+11v=109n.
\]

The bounds force \(m,n\in\{-1,0,1\}\). Their difference gives \(v=109n-89m\). Any nonzero choice has absolute value at least 20, contradicting \(|v|\le10\). Thus \(m=n=u=v=0\). ∎

Complementary information is not the same as independent evidence: both observations here share one source and one algebra. The theorem concerns joint identifiability, not independent scientific witnesses.

## 7. What this case teaches the method

The reusable sequence is: state the observed pattern exactly; build the algebra that generates it; test the proposed equivalence on a nontrivial kernel element; preserve the resulting counterexample; replace the failed global claim by a sharp domain-qualified theorem; then give a constructive inverse and the conditions needed to compose it safely.

Known-result recovery, a derived proof, finite computation, and historical novelty are separate labels. The displayed proofs are not made stronger by calling the example a breakthrough. The interesting gain is an explicit theorem where a metaphor previously stood.

## References and boundaries

Vanni Noferini and Gerald Williams, *Smith forms of matrices in Companion Rings, with group theoretic and topological applications*, arXiv:2408.08662v1, https://arxiv.org/html/2408.08662v1 .

David Harvey, *Faster polynomial multiplication via multipoint Kronecker substitution*, arXiv:0712.4046v1, https://arxiv.org/html/0712.4046v1 .

These establish relevant companion-ring and bounded-evaluation antecedents. No novelty priority is claimed for the individual constructions or this presentation. Nothing here proves a global assertion about zeta zeros, Collatz termination, prime-pair representations, or the ABC inequality. The result is a rigorous, reusable arithmetic transport with an explicitly qualified return path.
