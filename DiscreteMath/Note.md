### Set Operations

[Def]
> **Subset Definition**:
> $A \subset B \iff$ every element of $A$ belongs to set $B$.
> $A \not\subset B \iff$ there exists some element of $A$ that doesn't belong to $B$.

> **Power Set Definition**:
> $\mathcal{P}(A) := \\{ S : S \subset A \\}$ is called the power set of $A$.

[Deriv]
> **Cardinality of Power Set**:
> If $A = \\{1, 2, 3, \ldots, n\\}$, then $|\mathcal{P}(A)| = 2^{|A|}$.
> *Proof*: For each element, there are 2 choices (include/exclude), so $2^n$ total subsets.

[Def]
> **Basic Set Operations**:
> - Union: $A \cup B = \\{x : x \in A \lor x \in B\\}$
> - Intersection: $A \cap B = \\{x : x \in A \land x \in B\\}$
> - Difference: $A \setminus B = \\{x : x \in A \land x \notin B\\}$
> - Complement: $A^c = U \setminus A$ where $U$ is the universal set

[Deriv]
> **Distributive Laws**:
> 1. $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$
> 2. $A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$
> *Proof*: For (1), $x \in LHS \iff x \in A \land (x \in B \lor x \in C) \iff (x \in A \land x \in B) \lor (x \in A \land x \in C) \iff x \in RHS$

### Well Ordering Principle and Division Algorithm

[Def]
> **Division Algorithm**:
> For $a,b \in \mathbb{Z}$ ($b \neq 0$), $\exists! q,r \in \mathbb{Z}$ such that:
> $a = bq + r$ with $0 \leq r < |b|$

[Deriv]
> *Existence*:
> Consider $S = \\{a - bk \geq 0 : k \in \mathbb{Z}\\}$.
> By WOP, $S$ has minimal element $r = a - bq$.
> Show $0 \leq r < |b|$ by contradiction.

> *Uniqueness*:
> Suppose $a = bq_1 + r_1 = bq_2 + r_2$.
> Then $b(q_1-q_2) = r_2-r_1$.
> Since $|r_2-r_1| < |b|$, must have $q_1=q_2$ and $r_1=r_2$.

### Introduction to Logic

[Def]
> **Proposition**: A declarative sentence with definite truth value.
> **Logical Connectives**:
> - Negation: $\neg p$
> - Conjunction: $p \land q$
> - Disjunction: $p \lor q$
> - Implication: $p \rightarrow q$
> - Biconditional: $p \leftrightarrow q$

[Deriv]
> **Implication Equivalence**:
> $p \rightarrow q \equiv \neg p \lor q$
> *Proof*: Compare truth tables for both expressions.

> **De Morgan's Laws**:
> 1. $\neg(p \land q) \equiv \neg p \lor \neg q$
> 2. $\neg(p \lor q) \equiv \neg p \land \neg q$