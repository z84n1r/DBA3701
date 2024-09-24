java c
DBA3701 (DSC3214): Introduction to Optimization 
Homework 2 
Due: Sep 28, 2024 
1.  (15 marks) Find all extreme points in the following polyhedra:
(a) F = {(x1, x2, x3, x4) : x1 + x2 + 2/1x3 ≤ 1, x1, x2, x3, x4 ≥ 0};
(b) F = {(x1, x2, x3) : x1 − x2 ≤ 1, x2 − x3 ≤ 1, x3 ≤ 1, x1, x2, x3 ≥ 0};
(c)
2.  (10 marks) Consider the following optimization problem:
max   10x1 + 12x2  + 12x3  
s.t.    x1 + 2x2 + 2x3  ≤ 20  
2x1 + x2 + 2x3  ≤ 20  
2x1 + 2x2 + x3  ≤ 20 
x1 , x2 , x3  ≥ 0. 
(a) Write down the dual problem. 
(b)  Suppose the optimal solution to the primal problem is x1   = x2   =  x3   =  4. Solve the optimal solution to the dual problem using complementary slackness condition. 
3.  (15 marks) Portfolio Management Problem: Consider the following portfolio management problem. There are 100 stocks.  The expected return of stock i is ri  per dollar invested (which could be negative) and the total budget is b dollars, where b > 0. Ignoring the risk of the return, the problem of maximizing the total expected return is
where xi  denotes the amount of money invested in stock i.
(a) Write down the dual problem to the above linear programming problem.
(b) What is the optimal solution to the primal and the dual respectively? 
(c) Verify the solution you provided in (b) is indeed optimal using the weak duality.
4.  (20 marks) A potter manufacturer can make four different types of dining room service sets:  JJP English, Currier, Primrose, and Bluetail.  Furthermore, Primrose can be made by two different methods. Each set uses clay, enamel, dry room time, and kiln time, and results in a profit shown in Table 1.
Table 1: Profit and resources consumed for each productE C P1 P2 B Capacity Clay (lbs) 10 15 10 10 20 130 Enamel (lbs) 1 2 2 1 1 13 Dry room (hours) 3 1 6 6 3 45 Klin (hours) 2 4 2 5 3 23 Profit 51 102 66 66 89 The manufacturer is currently committed to making the same amount of Primrose using method 1 and method 2.  The formulation of the profit maximization problem is given below. The decision variables E,C, P1 , P2 , B are the number of sets of type English, Currier, Primrose Method 1, Primrose Method 2, and Bluetail, respectively. We assume, for the purposes of this problem, that the number of sets of each type can be fractional.
max   51E + 102C + 66P1  + 66P2  + 89B
s.t.    10E + 15C + 10P1  + 10P2  + 20B ≤ 130
E + 2C + 2P1 + P2 + B ≤ 13
3E + C + 6P1  + 6P2 + 3B ≤ 45
2E + 4C + 2P1 + 5P2 + 3B ≤ 23
P1  − P2  = 0
E,C, P1 , P2 , B ≥ 0.The optimal solution to the primal is given in Table 2 and the optimal solution to the dual together with sensitivity information is given in Table 3. Use the information to answer the questions that follow.
Table 2: The optimal solution to the primalOptimal Value Objective Coefficient E 0 51 C 2 102 P1 0 66 P2 0 66 B 5 89 
Table 3:  The optimal solution to the dual and the sensitivity.   The last two columns describe the ranges of b for which the optimal dual solution remains the sameDual Variable Const. RHS Allowable Increase Allowable Decrease Clay 1.429 130 153.33 86.25 Enamel 0 13 
∞ 9 Dry room 0 45 
∞ 17 Klin 20.143 23 28.60 19.50 Primrose Methods 11.429 0 3.50 0 
(a) What is the optimal quantity of each service set, and what is the total profit?
(b)  Give an economic interpretation of the optimal dual variables appearing in the sensitivity report, for each of the five constraints.
(c)  Should the manufacturer buy an additional 20 lbs.  of Clay at $1.1 per pound?
(d)  In the current model, the number of Primrose produced using method 1 was required to be the same as the number of Primrose produced by method 2. Consider a revision of the model in which this constraint is replaced by the constraint P1  − P2   ≥  0.   In the reformulated problem would the amount of Primrose made by method 1 be positive?
5.  (20 marks) Diet Problem: The “diet  problem”  concerns with finding a mix of foods that satisfies requirements on the am代 写DBA3701 (DSC3214): Introduction to Optimization Homework 2Python
代做程序编程语言ount of nutrition.  We consider here the problem of choosing fruits to meet certain nutritional requirements. The nutrition information of five selected fruits is provided in Table 4 along with a minimum required and maximum allowed intake of each type of nutrition in the last two columns. Your goal is to find the cheapest combination of fruits that will meet nutritional requirements.
(a)  Formulate a mathematical model for this problem. Solve the problem using Python and attach your code. Present and interpret the results.
Table 4: Nutrition and price information per 100 gramsApple Banana Blueberries Durian Tangerine Min Reqd Max Allowed Calories Carbohydrate (g) Fiber (g) Vitamin A (IU) Vitamin C (mg) 52 14 2.4 54 4.6 89 23 2.6 64 8.7 57 14 2.4 54 9.7 147 27 3.8 44 19.7 53 13 1.8 681 26.7 500 50 20 2000 75 3000 400 30 3500 150 Price (S$/100g) 0.5 0.3 2.5 10 0.5 
(b) Without solving the problem using the software, can you determine how your optimal solution and optimal spending in (a) will change if you are also con- cerned with the total fat intake.  The fat contained in each of the fruit and your nutrition requirement on fat is provided in the table below.  Verify your solution by solving the problem numerically.Apple Banana Blueberries Durian Tangerine Min Reqd Max Allowed Fat (g) 0.2 0.3                  0.3 5                  0.3 0 10 6.  (20 marks) Pricing Problem: Consider a retailer with an initial inventory of 2000 units of a single fashion item.  The retailer needs to sell his inventory over a time horizon of 15 weeks by employing in order the four price levels:  $60 (full price), $54 (90% discount), $48 (80% discount), $36 (60% discount) over time. The estimated average demands under these price levels are summarized in the following table.
Any left over items at the end of the selling season can be sold to outlet for $25 per
Table 5: Estimated demand under each price
Price $60 $54 $48 $36 
Demand 125 162.5 217.5 348.8 unit (salvage value). The retailer is required to start with the full price for at least one week and then he is allowed to decrease his prices over time. The retailer seeks to maximize the total revenue during the selling horizon (including salvage value) by determining the timing and magnitude of the markdowns.  Answer the following questions and attach the codes you used to derive the solutions.
(a) Formulate the problem as a linear program and report your solution.  (Hint: Let xi  be the number of weeks that price i,i = 1, 2, 3, 4 is used, and we allow fractional weeks here.)
(b) What is the shadow price associated with the initial inventory level?  Resolve your model by increase the initial inventory level to 2001.  Does your profit increase by the same amount as the shadow price indicated? Explain why.
(c)  Suppose in order to maintain the brand reputation, the retailer is only allowed to discount from week 4.  Will the retailer change his markdown strategy in this case?
(d) In the traditional brick-and-mortar business, menu cost and consumer price impression are the two major reasons behind the very few number of price levels. With the rise of e-commerce and other technologies, it is possible for the retailer to employ more price levels and change the price more frequently. In the above problem, what happens if the retailer employs the following price grids (with a grid of $2) instead of a few discount levels?  For simplicity, the demand estimates at the additional price levels are taken as a linear interpolation of the original demands (see the table below).  What is the improvement in revenue compared to the benchmark?  What is the new markdown policy?  How do you compare with the original policy?
Table 6: Price grids model 
Price        $60    $58    $56     $54      $52     $50      $48     $46      $44      $42     $40     $38    $36
Demand   125   137.5   150   162.5   180.8   199.1   217.5   239.4   261.3   283.2   305.1   327   348.8



         
加QQ：99515681  WX：codinghelp
