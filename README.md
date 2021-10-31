BL40A2010 Introduction to IoT-Based Systems
Assignment 6,29.10.2021
Author:ZhouZiao
Prisoner's dilemma is a standard example of a game analyzed in game theory that shows why two completely rational individuals might not cooperate, even if it appears that it is in their best interests to do so. It was originally framed by Merrill Flood and Melvin Dresher while working at RAND in 1950. Albert W. Tucker formalized the game with prison sentence rewards and named it "prisoner's dilemma", presenting it as follows:

"Two members of a criminal gang are arrested and imprisoned. Each prisoner is in solitary confinement with no means of communicating with the other. The prosecutors lack sufficient evidence to convict the pair on the principal charge, but they have enough to convict both on a lesser charge. Simultaneously, the prosecutors offer each prisoner a bargain. Each prisoner is given the opportunity either to betray the other by testifying that the other committed the crime, or to cooperate with the other by remaining silent. The possible outcomes are:

If A and B each betray the other (not-cooperating to each other), each of them serves $z$ years in prison (payoff of $-z$)
If A betrays B (not-cooperating with B) but B remains silent (cooperating with A), A will serve $y$ years in prison (payoff $-y$) and B will serve $w$ years (payoff of $-w$).
If B betrays A (not-cooperating with A) but A remains silent (cooperating with B), B will serve $y$ years in prison (payoff $-y$) and A will serve $w$ years (payoff of $-w$).
If A and B both remain silent, both of them will serve $x$ years in prison (payoff of $-x$)."
The payoff table is presented below.

$B$ cooperates	$B$ not-cooperating
$A$ cooperates	$A \rightarrow -x$	$A\rightarrow -w$
$B\rightarrow -x$	$B\rightarrow -y$
$A$ not-cooperating	$A\rightarrow -y$	$A\rightarrow -z$
$B\rightarrow -w$	$B\rightarrow -z$
However, this is only a Prisoner's Dilemma GAME for A GIVEN RELATION between the years in prison (payoffs) as to be studied next.

ps. Text adapted from Wikipedia.

(1) Consider the Prisoner's dilemma description given above.

(a) What is the relation between the payoffs values $x\geq 0$, $y\geq 0$, $w\geq 0$ and $z \geq 0$ so that the game can be classified as Prisoner's Dilemma?

the relation between the payoffs values is 0 ≤ y < x < z < w
(b) Verify the results (i.e., the proposed inequality) with numerical examples using nashpy. Please provide one example when the inequality holds and one it does not (check my example for Dove and Hawyk game).

![9a10a98de8c330e69437f22da32c5f1](https://user-images.githubusercontent.com/91326706/139581415-e178787f-92c9-4f21-ab35-fa2f095af46c.png)
![f42281aaa005fcadd708c76ef255faf](https://user-images.githubusercontent.com/91326706/139581417-b1b53103-0dae-46c5-900c-a62eb30f8b9d.png)
![image](https://user-images.githubusercontent.com/91326706/139581441-832c6304-67d5-40e6-a608-da2e8bddd1c5.png)
![image](https://user-images.githubusercontent.com/91326706/139581452-5fc1d5b4-de45-45a2-b8f8-20e5c33cded1.png)


(2) Justify why the game from the previous exercise is or is not a good (reasonable) model when $A$ and $B$ are:

1. Two trained members from the army when they are in prison.

2. Competitive companies in the market discussing standardization.

3. Two different autonomous IoT-based home energy management algorithms that are focus on energy efficiency.

4. Two different autonomous IoT-based home energy management algorithms that are focus on profit maximization.

ps. You need to think about the assumption used in Game Theory and in the Prisoner's dilemma problem setting.

Answer:
1. No, the two trained menbers do not affect each other.
2. Yes, in order to take predominate in market shares,They will betray each other, even if they
can share the market equally through cooperation.
3. No, since they can work in cooperation and have the same shared goal. The energy efficiency
of house A does not affect the payoff of house B.
4. Probably no, But it can also be yes if they are competing for the same resource and decisions
of A and B may affect each other.
