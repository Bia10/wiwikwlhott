General FAQ
====================================================

What is the point of constructive mathematics?
----------------------------------------------------------------------------------------

.. epigraph::

    Constructive mathematics is in its infancy.  According to some, it
    is doomed to the role of scavenger.  These people conceive of
    classical mathematics as establishing the grand design and the
    imaginative insight, leaving the constructivists to add whatever
    embellishments their credos demand.  Although totally wrong, this
    viewpoint hints at a truth: The most urgent task of the
    constructivist is to give predictive embodiment to the ideas and
    techniques of classical mathematics.  Classical mathematics is not
    totally divorced from reality.  On the contrayr, most of it has a
    strongly constructive cast.  Much of the constructivization of
    classical mathematics is therefore routine; constructive versions
    of many standard results are readily at hand.  This makes it easy
    to miss the point, which is *not* to find a constructive version
    of this or that, or even of every, classical result.  The point is
    not even to find elegant substitutes for whole classical theories.
    The point rather is to use classical mathematics, at least
    initially, as a guide.  Much will be of little value to the
    constructivist, much will be constructive per se, and much will
    raise fundamental questions which classically are trivial or
    perhaps do not even make sense. The emphasis will be on the
    discovery of useful and incisive numerical information.  It is the
    incisiveness and scope of the information, not the elegencae of
    the format, that is relevant.

    -- Bishop :cite:`bishop:numerical:language`

Truncation: classical or constructive?
-------------------------------------------------

One understanding of the term "constructivism" is that the logic
should always pass around explicit constructions, which may in general
not be unique.  So existential quantifiers are understood to always be
proved by constructing points, and logical disjunctions are understood
to always give a choice of a disjunct.

From this point of view, the truncation operation seems to be
non-constructive: indeed, it allows us to pass around a notion of
truth without passing around the underlying witnesses.  There are (at
least) two problems with this conclusion.

- This understanding of constructivism is correct only for certain
  variants of constructivism.
- Perhaps more importantly, witnesses *are* passed around.

For the latter, define the type :math:`P` of primes numbers that are
the sum of two consecutive primes.  Then it can be shown that
:math:`P` is a proposition: any two of its elements are equal.
Moreover, :math:`P` is inhabited, namely by the number 5, being the
sum of 2 and 3.  But the proof of :math:`P` is indeed very
informative: for example, the first projection of *any* proof of
:math:`P` will yield the number 5.

Another striking example of elements of truncated types carrying data
is given by Nicolai Kraus' function that undoes the truncation map
:math:`|\,\cdot\,|:\mathbb{N}\to\|\mathbb{N}\|`
:cite:`kraus:truncation:invertible`.  In this construction, for any
natural :math:`n:\mathbb{N}`, we consider the type
:math:`\operatorname{pathto}(\mathbb{N},n)` of :term:`pointed types`
equal to the pointed type :math:`(\mathbb{N},n)`.
:math:`\operatorname{pathto}(\mathbb{N},n)` is then seen to be a
proposition, which allows us to extract the incoming point :math:`n`,
even if it was hidden by the truncation map :math:`|\,\cdot\,|`.

What is the killer application of univalence?
------------------------------------------------

NB: The following answer is opinionated.

If one restricts one's attention to sets only, and disregards things
like higher-inductive types as artificial, then it seems that function
extensionality and propositional extensionality together suffice for
the vast majority of mathematics.  Hence, it is quite difficult to
convince someone, who is only interested in sets, of the importance of
univalence, as they will never need it.  On the other hand, it is only
*through* univalence that one naturally encounters types that are not
sets, namely universes.  However, the motivation for univalence is not
circular:

Univalence has been, and continues to be, very informative for
developing intuition in type theory.  It is often possible to obtain
intuition from univalence, and make an initial estimate whether some
claim is going to be provable or not.  Even if your entire theory can
be built in MLTT, univalence can guide you.

.. todo:: add an example of this intuition obtained from univalence

So let me say at least this: *if* one is interested in arbitrary
types, rather than restricting to sets, univalence leads the way,
either directly or indirectly.

.. todo:: Is this all we can say?  This answer seems a bit
          incoherent...  "What is the final answer?"