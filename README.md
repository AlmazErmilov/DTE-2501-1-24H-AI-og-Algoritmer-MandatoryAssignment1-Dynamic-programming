# DTE-2501-1-24H-AI-og-Algoritmer-MandatoryAssignment1-Dynamic-programming

## Problem description

The task is to find the minimum number of coins to make 1,040,528 NOK using Norwegian coins with denominations of 1, 5, 10, and 20 NOK.

## Approaches

2 methods were used to solve this problem:
1. Greedy algorithm
2. Dynamic programming

### Greedy approach

Steps:
1. Sort coins from highest to lowest value
2. Use the highest value coin possible at each step
3. Keep a count of coins used

Result:
- Total coins: 52 030
- Coins used: 52 026 x 20 NOK, 1 x 5 NOK, 3 x 1 NOK

### Dynamic programming approach

This method breaks the problem into smaller subproblems. For each amount from 1 to 1,040,528 NOK, calculate the minimum number of coins needed

Result is that minimum number of coins for 1,040,528 NOK: 52,030

## Discussions

### Coin Value per Unit

- 20 NOK coin: 20.0 value per coin
- 10 NOK coin: 10.0 value per coin
- 5 NOK coin: 5.0 value per coin
- 1 NOK coin: 1.0 value per coin

Higher denomination coins have higher value per unit, aligning with the greedy approach of using the highest value coins first.

### Comparison of approaches

Both methods produced the same result: 52 030 coins. It seems that it happens because of the specific properties of the Norwegian coin system.
The greedy method works best for these coins because of how they're set up. each coin is either a multiple of smaller coins, or it's just one more than what you can make with smaller coins. this means that always picking the biggest coin you can use will give you the best answer. 

The same results between greedy and dynamic programming approaches would not be the same for all coin systems. In many cases, the greedy approach may yield suboptimal solutions.

One example where the approaches differ:
- Coins: {1, 15, 25}
- Target sum: 30
- Greedy solution: 25 + 5x1 = 6 coins
- Optimal solution: 2x15 = 2 coins

## Conclusion

Both greedy and dynamic programming approaches gave the optimal solution (52 030 coins) for the Norwegian coin system. The dynamic programming solution is more valuable as it gives the optimal solution for any coin system making it more versatile.
