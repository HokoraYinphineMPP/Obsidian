# Course Summary
## Statements
-   **MO1**. Understand and identify mathematical statements.
-   **MO2**. Construct molecular statements using the logical connectives: conjuction, disjunction, implication, biconditional, and negation. 
-   **MO3**. Identify the hypothesis and conclusion in an implication and understand the truthness/falsity of implications.  
-   **MO4**. Construct the converse and contrapositive of implications.  
-   **MO5**. Translate between English-language statements and symbolic logic.  

### Warm up
A high-performance computing cluster is controlled by two servers: compute and file, and the cluster cooling system consists of three units. The cluster admin recieved three diagnostic messages by email:
1. Bad file server, and the first cooling unit;
2. Bad compute server, and the second cooling unit;
3. File server is normal, but bad third cooling unit;

Only one server and no more than one cooling unit are bad
After repair it turned out that each message contained valid information either about the server's operation or about the cooling units' condition, but not simultaneously. Which server and which cooling units did the admin have to repair?

###### Work Process
|fc|123|
|:-:|:-:|
|tf-ttf|2|
|tf-tft|3|
|tf-ftt|123|
|ft-ttf|13|
|ft-tft|12|
|ft-ftt| |

1. Bad file server, and the first cooling unit is good;
2. Bad compute server, and the second cooling unit is good;
3. File server is normal, third cooling unit is good;

###### Answer
he had to fix compute server and 1st cooling unit



|P|Q|P→Q|~P|~P∨Q|
|:-:|:-:|:-:|:-:|:-:|
|t|t|t|f|f|
|t|f|f|f|f|
|f|t|t|t|t|
|f|f|t|t|t|
~(P→Q)=~(~P∨Q)
=(~(~P))∧(~Q)
P∧(~Q)

C→B
If cow, then beans
C→~B=~C∨~B
~B→~C=C→B `contrapositive`
B→C
~C→~B `inverse`
C∧~B=~(~C∨B)
=~(C→B)


### Statements
A __Statement__ is a sentence that is either `True` or `False`
Ex:
|Examples|T/F|
|:-|:-:|
|$p:"5>2"$|True|
|$q:"2>5"$|False|
|$r:"x>2"$|Not a statement|
###### New statement from old
|p q|def|
|:-:|:-:|
|~p|not p|
|p∧q|p and q|
|p∨q|p or q|
ie:
`my shirt is gray but my shorts are not`
`my shirt is gray` = p
`my shorts are gray` = q
`my shorts are not gray` = ~q
`but` = ∧
p∧~q

### Conditional Statements
Def: p→q means:
"if p is TRUE then q is TRUE"
|p|q|p→q|
|:-:|:-:|:-:|
|T|T|T|
|T|F|F|
|F|T|T|
|F|F|T|

ie:
`If I study hard, then I will pass`
`I study hard` = p
`I will pass` = q
if p then q
p→q
`either I don't study hard, or I pass`
`I don't study hard` = ~p
`I pass` = q
`or` = ∨
~p∨q

### Types of Statements
|Type|p→q|
|:-:|:-:|
|Conditional|p→q|
|Converse|q→p|
|Inverse|~p→~q|
|Contrapositive|~q→~p|
|Biconditional|p⇔q|
Note: Conditional and Contrapositive have the same truth value
Note: Converse and Inverse have the same truth value
- ⇔ means: "If and only if" aka "iff"
it means if p is true, then q is true, and vice versa

ie:
`If you study, then you will get a good grade`
`you study` = p
`you will get a good grade` = q
p→q
Converse: `If you get a good grade, then you studied`
Inverse: `If you do not study, then you will not get a good grade`
Contrapositive: `If you did not get a good grade, then you did not study`


## Set Theory
-   **MO1**. Perform set-theoretic operations including listing elements, set roster notation, and set-builder notation. 
-   **MO2**. Distinguish between members of sets and subsets. 
-   **MO3**. Perform set-theoretic computations including union, intersection, complement, product, and cardinality. 

### Warmup 

#### Q2
Dana says they have 10 toys
Milla says 8 toys
Milla stole at least 1 toy while dana is using 1 toy

Milla: 9-17
Dana: 1-9

#### Q3
###### if $C$ is the set of all students in our class today, is your group a subset or an element?

Subset

###### if $G$ is the set of all members of your group today, what are the elements of $G$?

Each person in our group

###### suppose $G$ is still the same set. how many subset of G are there?

possibly infinite, but currently none

###### What is $G\cap C$? $G\cup C$?
$\cap$ represents all elements that are in both G and C (intersect)
$\cup$ represents all elements in both G and C (union)

#### Q4
###### Find the following cardinalities
- $|A|$ when $A=\{6,7,8,9,...,29\}$
23 elements

- $|A|$ when $A=\{z\in \mathbb{Z}|-4\leq z\leq 95 \}$
100 elements

- $|A\cap B|$ when $A=\{x\in \mathbb{N} |x\leq 25\}$ and $B=\{z\in \mathbb{N}|z$ is prime$\}$
9 elements


#### Q5
###### Find a set of smallest possible size that has both $\{1,3,5,6,10\}$ and $\{1,2,6,8,10\}$ as subsets.
$\{1,2,3,5,6,8,10\}$

#### Q6
###### Let $A=\{0,3,7,8,15\}$ and $B=\{3,7,15\}$. How many sets $C$ satisfy $C\subseteq A$ and $B\subseteq C$?
$\{3,7,15\}$
$\{0,3,7,15\}$
$\{3,7,8,15\}$
$\{0,3,7,8,15\}$
4 elements

#### Q7
###### Let $A=\{1,3,5\}$ and $B=\{2,3\}$. What are all the elements of $A\times B$ and $B\times A$? Is $A\times B=B\times A$?
$A\times B=\{(1,2),(1,3),(3,2),(3,3),(5,2),(5,3)\}$
$B\times A=\{(2,1),(2,3),(2,5),(3,1),(3,3),(3,5)\}$
No, because the ordered pairs are not the same order

#### Q8
###### Draw a Venn Diagram representing the two sets $\overline{A\cap B}$ and $\overline{A}\cup \overline{B}$. What do you notice about $\overline{A\cup B}$ and $\overline{A}\cap \overline{B}$?
![[Pasted image 20220830170206.png]]

## Functions
-   **MO1**. Understand the definition of a function including domain, codomain, image, range, and ways of defining functions. 
-   **MO2**. Compute outputs of recursively defined functions. 
-   **MO3**. Determine if a function satisfies the 

###
###### $$|A\cup B\cup C|=|A|+|B|+|C|-|A\cap B|-|A\cap C|-|B\cap C|+|A\cap B\cap C|$$
## Counting Problems
-   **MO1**. Apply the additive principle to solve counting problems. 
-   **MO2**. Apply the multiplicative principle to solve counting problems. 
-   **MO3**. Apply the principle of inclusion and exclusion to solve counting problems. 

### Subsets
$(_{k}^{n})= \textrm {num of ways to pick k from n}$
4 employees, team of 2
$7*6*5/6$

###### $$(_{k}^{n})=C(n,k)=_nC_k=\frac{n!}{(n-k)!k!}$$
The number of subsets of a set of size $n$ each with cardinatily $k$
###### $$P(n,k)=_nP_k=\frac{n!}{(n-k)!}$$
###### $$|\mathcal{P}(A)|=2^n$$
Where $n$ is the number of elements in $A$


###### $A.B.C.D.E$
###### $$5*4=\frac{5!}{(5-2)!}=\frac{5*4*3!}{3!}=5*4$$

6 students in row 1
arrange 3
$P(6,3)$ or (Choose 3 from 6)\*(order the 3 we picked)
$P(6,3)=\frac{6!}{(6-3)!}$
$\frac{6!}{(6-3)!}3!$


n students in row 1
arrange k
$P(n,k)$ or (Choose k from n)\*(order the k we picked)
$P^n_k=\frac{n!}{(n-k)!}$
$\frac{n!}{(n-k)!k!}$