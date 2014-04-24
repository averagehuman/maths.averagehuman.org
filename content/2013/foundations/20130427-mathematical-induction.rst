
Mathematical Induction
======================

:date: 2013-04-27
:author: averagehuman
:category: Foundations
:latex:

Scientific Inference
--------------------

In any scientific discussion it might be said that **deduction** and **induction** are
the the most prominent methods of logical reasoning. Deduction is the method that
progresses from the general to the particular, and induction the method that
progresses from the particular to the general. In other words, given a theory
which has been proved to be true (or is accepted as being axiomatically true),
one may logically **deduce** that there are other facts which must
be true in consequence - given *A* it is obvious or demonstrable that *B*.
Alternatively, given a collection of measured facts or phenomena, one may
logically **induce** (or infer) that there is a Law of the Universe "governing" these
facts or phenomena, in the sense that, if the proposed Law did not hold,
then the facts or phenomena *as a collection* would not have occurred.
One notable difference between the two forms of reasoning is that a deductive
argument can be proved or disproved, but an inductive argument can only
be disproved since, no matter how many facts are gathered supporting a
thesis, there is always the possibility of new evidence which goes against
it. (But see `The Problem of Induction`_ for philosophical objections)

Mathematical Induction
----------------------

Mathematical Induction has a stricter definition and shouldn't be confused
with the more general scientific method. The best informal description is as a
line of dominos - given a line of up-ended dominos, if you can show that:

1. the first domino must fall
2. if **any** one of the dominos fall, then the next domino (its successor)
   will also fall

then you can say with certainty that `all the dominos must fall`.

The "line of dominos" here is in fact some general assertion involving some
sequence of mathematical statements.  For example, to assert the truth of the
binomial theorem:

.. math::

    (x + y)^n = \sum_{i=0}^{n} {n \choose i} x^iy^{n-i}, n = 0, 1, 2, \dots

is to assert the truth of each item of the sequence:

.. math::

    \begin{array}
    \\
    (x + y)^0 &= \sum_{i=0}^{0} {0 \choose i} x^iy^{0-i} \\
    (x + y)^1 &= \sum_{i=0}^{1} {1 \choose i} x^iy^{1-i} \\
    (x + y)^2 &= \sum_{i=0}^{2} {2 \choose i} x^iy^{2-i} \\
    \end{array}

and so on. So if you can:

1. Show that the first item in the sequence is true (when \\(n = 0\\))
2. Show that **IF** the \\(k\\)th item in the sequence is true, then
   the \\(k + 1\\)th case must also be true

then it can be said that the proposed theorem is true for all \\(n \\in \\mathbb{N} \\).

More formally, this *Principle of Induction* can be stated:

.. container:: panel highlight

    .. math::

        P(0) \wedge \left(\forall k \in \mathbb{N} [P(k) \Rightarrow P(k+1)]\right) \Rightarrow \forall n \in \mathbb{N} [P(n)]

where `P` is any proposition.

This can simply be accepted as an axiom but, if it helps you to sleep better,
there are set-theoretic proofs based on the `well-ordering`_ of the natural
numbers \\(\\mathbb{N}\\), for example,
`here <http://www.proofwiki.org/wiki/Equivalence_of_Well-Ordering_Principle_and_Induction>`_
[proofwiki.org].

Strong Induction
~~~~~~~~~~~~~~~~

The two parts of an Inductive proof are the **base case** and the **inductive
step**. The base case is, as stated, the proof of the given statement for the
first item in the sequence - typically when \\(n = 0\\) but, in general, when
\\(n\\) is some lowest positive integer. And the inductive step is the assumption
of the \\(k\\)th case and the subsequent proof of the \\(k+1\\)th case.

It may be the case that assumption of the \\(k\\)th case is insufficient in
achieving the inductive step, and so invoking **strong induction** is called
for. With strong induction you assume, not just the `kth` case, but each case
up to and including the `kth`.

:see also: `Wikipedia`_, `NRICH`_, `The Method of Descent`_

.. _The Problem of Induction: https://en.wikipedia.org/wiki/Problem_of_induction
.. _well-ordering: https://en.wikipedia.org/wiki/Well-order
.. _Wikipedia: https://en.wikipedia.org/wiki/Mathematical_induction
.. _NRICH: http://nrich.maths.org/4718
.. _The Method of Descent: http://mathcircle.berkeley.edu/BMC4/Handouts/induct/node7.html



