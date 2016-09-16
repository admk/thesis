Page 19
=======

Adds a definition for ``semantics``.


Page 30
=======

``Variable-precision DSP`` is now ``fracturable DSP``.


Page 37
=======

Figure 2.5 is now updated to reflect the requirement to read only once per
cycle.


Page 51
=======

Reiterates the high-level intuition for why we desire the most precise solution
from solving the fixpoint equation.

Defines what $\varnothing$ is.  (An empty set.)


Page 53
=======

Adds a missing definition for ``complete lattice``.


Page 55
=======

::
    Widening and narrowing operators can be used to reduce the number of
    iterations required to reach a fixpoint...

Replaces ``to reach a fixpoint`` with ``in the iterative computation steps`` to
avoid confusion.  A ``fixpoint`` in this context is not incorrect, but a bit
misleading because it is slightly different than (2.21) introduced earlier.


Page 57
=======

Potential confusion about (2.35) is now fixed with a worked example and a
sentence to reiterate the rationale of abstraction.

A definition is also provided for the pair $\underline{X^\sharp}$ and
$\overline{X^\sharp}$.


Page 58
=======

The explanation for $s \circ t$ has been rewritten.


Page 59
=======

Ambiguity mentioned during viva about the following.

::
    This is because intervals can only imply inequalities of the latter form,
    $\pm x \leq c$, but not the former, $x - y \leq c$.
::
    ... introduces a perturbation on the constant $\alpha_0^x$.


Page 60
=======

Explains the partial order operations is defined for the abstract error domain.


Page 71
=======

Fixes the following ambiguity mentioned during viva.  It is now clear that
transformations are performed and appended on an E-PEG.

::
    By repeatedly applying all possible passes...


Page 80
=======

Clears the confusion about $\hat{v}_+$ and $v_+$ as both of them are not
defined previously, when $\hat{v}_i$ and $v_i$ are intended.  Additionally,
$\hat{v}_i$ and $v_i$ are now also defined.

::
    The error between $x = \hat{v}_+$ and $y = v_+$ is defined as follows...


Page 82
=======

Reiterates the reason why the third alternative in (2.58) is not equivalent to
the other two.  (Because series expansion is applied.)


Page 87
=======

Fixes the offset values in the definition of the IEEE 754 format in both (3.1)
and (3.2).  Also adds the definition of gradual and abrupt underflows, and how
``ulp`` can be computed in each case.


Page 91
=======

Explains why our simple resource estimation is accurate.  (Because
floating-point data-paths do not exhibit much cross-module optimization.)


Page 96
=======

Explains how the number of equivalent expressions that can be discovered scales
with $k$, which is not very scalable.


Page 98
=======

Mentions the meaning of the function $\mathsf{fr}$.  (The Pareto frontier
algorithm.)


Page 105
========

Discusses the fact that DSP count increases linearly with the estimated LUT
count.  Again mention the lack of scalability of $k$ and this to be solved in
later chapters.


Page 117
========

::
    It expresses how each program variable is updated, but abstracts away the
    order in which the updates occur, and ignores any temporary variables that
    are not marked as program outputs.

Jason asked about whether the order affects accuracy.  The texts now clarifies
that the order of arithmetic computations not affected in the translation to
MIR, in the sense that control- and data-flow of the original program are still
preserved.


Page 120
========

Mentions that $\mu_1$ is always evaluated before $\mu_2$ in $\mu_2 \star
\mu_1$.


Page 137
========

Fixes spacing in (4.37) to avoid confusion in expressions because of ambiguous
operator precedence.


Page 141
========

Provides rationale for performing simulation.  (To prove a strong correlation
between the reduction of analyzed round-off errors to that of actual errors
during execution.)


Page 144
========

Adds shortcomings of this chapter addressed in the next chapter:
  * Long optimization time
    - Prohibits greater partial loop unrolling depths
    - Hinders better accuracy improvements
  * Simple resource estimation without temporal sharing
    - Significant increase in the resource requirements of optimized circuits


Page 155
========

Clarifies that the lack of referential transparency indicates side-effects may
present.


Page 182
========

Explains the shortcoming in scalability in ``other practical considerations``.
