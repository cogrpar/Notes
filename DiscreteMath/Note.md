<<<<<<< HEAD
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
=======
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

### Proof Techniques & Quantifiers

[Def]  
> **Quantifier Definitions**:  
> - Universal: $\\forall x \\in S, P(x) \\equiv P(x\_1) \\land P(x\_2) \\land \\dots$  
> - Existential: $\\exists x \\in S, P(x) \\equiv P(x\_1) \\lor P(x\_2) \\lor \\dots$  

[Deriv]  
> **Quantifier Negation**:  
> 1. $\\neg(\\forall x \\in A, P(x)) \\equiv \\exists x \\in A, \\neg P(x)$  
> 2. $\\neg(\\exists x \\in A, P(x)) \\equiv \\forall x \\in A, \\neg P(x)$  

> **Nested Quantifiers**:  
> $\\forall x \\in A, (\\forall y \\in B, P(x,y)) \\equiv \\forall y \\in B, (\\forall x \\in A, P(x,y))$  

### Example: Zero Product Property
Show $\\forall a,b \\in \\mathbb{Z}, (ab=0) \\rightarrow (a=0 \\lor b=0)$
<details>
<summary>Click for Solution</summary>

1. **Rewrite Implication**:  
   $ab=0 \\rightarrow (a=0 \\lor b=0) \\equiv \\neg(ab=0) \\lor (a=0 \\lor b=0)$  

2. **Proof by Contrapositive**:  
   Assume $a \\neq 0 \\land b \\neq 0$, then $ab \\neq 0$.
</details>

[Deriv]  
> **Quantifier Distribution Laws**:  
> - $\\forall x\\, (P(x) \\land Q(x)) \\equiv (\\forall x\\, P(x)) \\land (\\forall x\\, Q(x))$  
> - $\\exists x\\, (P(x) \\lor Q(x)) \\equiv (\\exists x\\, P(x)) \\lor (\\exists x\\, Q(x))$  

> **Non-Distributive Cases**:  
> - $\\forall x\\, P(x) \\lor Q(x) \\not\\equiv (\\forall x\\, P(x)) \\lor (\\forall x\\, Q(x))$  

### Statement Translation Guide
[Def]  
> **Formalization Rules**:  
> 1. "Every X satisfies P" $\Rightarrow$ $\\forall x\\, P(x)$  
> 2. "There exists an X with P" $\Rightarrow$ $\\exists x\\, P(x)$  
> 3. "Infinitely many X" $\Rightarrow$ $\\forall n\\, \\exists x>n\\, P(x)$  

**Examples**:
1. **Goldbach's Conjecture**:  
   $\\forall n \\in \\mathbb{Z}\_{>2}\\, (\\text{Even}(n) \\rightarrow \\exists p,q \\in \\text{Primes}\\, p+q=n)$

2. **Twin Prime Conjecture**:  
   $\\forall N \\in \\mathbb{N}\\, \\exists p>N\\, (\\text{Prime}(p) \\land \\text{Prime}(p+2))$

3. **Fermat's Last Theorem**:  
   $\\forall n \\in \\mathbb{Z}\_{>2}\\, \\neg \\exists x,y,z \\in \\mathbb{Z}\_{>0}\\, x^n+y^n=z^n$
>>>>>>> 3d8afd8078e52e8c7d95897ad5916385f9f4e181
