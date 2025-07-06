**Probability** is a way to measure how likely something is to happen.

The **sample space** is the list of _all possible results_. Imagine you’re rolling a normal 6-sided die. Then **Sample Space (S) = {1, 2, 3, 4, 5, 6}**

An **event** is a specific outcome (or group of outcomes) from the sample space.
- **Example 1:** _"Getting an even number"_  
    → Possible outcomes: {2, 4, 6}  
    → This is an **event**.

Basic rules:
1. Complement rule: The probability of not happening. P(not A) = 1 - P(A)
2. Additional rule: This rule is to calculate the probability of happening **either Event A OR Event B**
	**Case 1: Mutually Exclusive (No Overlap)**
	_(Example: Rolling a die → Can’t be both 2 and 5 at the same time.)_
	**Formula:**
	P(A OR B)=P(A)+P(B)
	**Example:**
	- P(Rolling a 2 or 5) = 1/6+1/6=2/6=1/3​.
	    
	**Case 2: Non-Mutually Exclusive (Overlap Possible)**
	_(Example: Drawing a card → Can be both a Heart and a King.)_
	**Formula:**
	P(A OR B)=P(A)+P(B)−P(A AND B)
	**Example:**
	- P(Heart OR King) = 13/52+4/52−1/52​=16/52​.  
	    _(Subtract the King of Hearts since it was counted twice!)_
3. Multiplication rule: This rule is to calculate that **both Event A AND Event B** happen.
   **Case 1: Independent Events**
   _(Example: Flipping a coin twice → First flip doesn’t affect the second.)_
   P(A AND B)=P(A)×P(B)
   eg: P(Head on 1st and Heads on 2nd flip) = 1/2 * 1/2 = 1/4
   **Case 2: Dependent Events**
   _(Example: Drawing cards without replacement → Second draw depends on the first.)"**Without replacement**" means that when you take an item from a group, you **do not put it back** before you take the next one._
   P(A AND B)=P(A)×P(B after A)
   eg: A bag has 3 red and 2 blue marbles. P(1st is red AND 2nd is blue) = 3/5 * 2/4 = 6/20[Total number of marble reduced as it was drawn without replacement]


### **Quick Summary Table**

|**Rule**|**When to Use**|**Formula**|
|---|---|---|
|**Complement**|Finding "not happening" probability|1−P(A)1−P(A)|
|**Addition (OR)**|"Either A or B" happens|P(A)+P(B)P(A)+P(B) (if no overlap)  <br>P(A)+P(B)−P(A AND B)P(A)+P(B)−P(A AND B) (if overlap)|
|**Multiplication (AND)**|"Both A and B" happen|P(A)×P(B)P(A)×P(B) (if independent)  <br>P(A)×P(B after A)P(A)×P(B after A) (if dependent)|

### **Conditional Probability**
Conditional probability tells us the chance of an event happening **given that another event has already happened**. It adjusts probabilities based on **new information**.
**Question:**  
_If you pick a red marble first and don’t put it back, what’s the probability the next marble is blue?_\
1. **First pick:** You took 1 red marble out.
    - Now, the bag has **4 red** and **3 blue marbles left**.
2. **Second pick:**
    - Total marbles left = 4 (red) + 3 (blue) = **7 marbles**.
    - Probability of blue now = 3/7​.

This is **conditional probability** because the chance of blue **depends on red being picked first**.

**Formula**
P(B∣A)=P(A AND B)/P(A)
- P(B∣A) = Probability of B **given** A happened.
- P(A AND B) = Probability of **both** A and B happening.
- P(A) = Probability of A happening.

### **Independence of Events**
Two events (**A** and **B**) are **independent** if:
- **One event happening does NOT affect the probability of the other.**
- In other words, knowing that **A** happened tells you **nothing** about whether **B** will happen.
##### **Examples of Independent Events**
✅ **Coin Flips:**
- First flip: **Heads**
- Second flip: Still **50% Heads** (unaffected by the first flip).

✅ **Dice Rolls:**
- Rolling a **4** on the first die doesn’t change the chance of rolling a **2** on the second die.

### **Bayes' Theorem Explained**
Bayes' Theorem is like a "probability updater" - it helps us adjust our beliefs when we get new information.
