# The-2025-IMC-Global-Trading-Challenge

This repository contains my personal reflections and contributions from the 2025 IMC Prosperity Trading Challenge, where I competed as part of **Team Jain Street** with fellow students from the UCLA Master of Financial Engineering program.

🔗 [View the leaderboard](https://prosperity.imc.com/leaderboard)

<img width="468" alt="image" src="https://github.com/user-attachments/assets/1bde4cd2-04a5-48cb-931b-8b8fc20ab51a" />

---

## About the Challenge

In April 2025, I participated in the IMC Prosperity Trading Challenge alongside four classmates. Competing under the team name **Jain Street**, we placed **138th overall** and **78th in the manual challenge**. The challenge consisted of five rounds and tested both our quantitative trading strategies and our ability to collaborate under pressure.

---

## Algorithmic Challenge and My Contribution

For the algorithmic portion, we divided the newly introduced products among team members for analysis and strategy development. One of my key contributions was the development of a trading strategy for the **Magnificent Macaron**, introduced in Round 4.

### The Magnificent Macaron Strategy

Macaron prices were influenced by:
- Sunlight index
- Sugar prices
- Shipping costs
- Tariffs and storage availability

The IMC provided a key hint suggesting a **Critical Sunlight Index (CSI)** that significantly impacted macaron and sugar prices.

### My Hypothesis:
Using price and sunlight data over four trading days, I plotted:
- The Island Mid Price of Macarons (blue line)
- The Sunlight Index (dashed gold line)

From the graph, I hypothesized:
- **CSI = 45**
- **Fair Value of Macarons ≈ 634 seashells**

![image](https://github.com/user-attachments/assets/665c1f3c-99a7-475f-8f40-8ee1c854d534)


### Strategy Implementation:
- Buy macarons when the Sunlight Index < 45
- Sell when the slope of the index changes from negative to positive

This strategy generated approximately **14,000 seashells** in the trading optimizer. However, it **failed to produce stable profits in the real testing environment**, highlighting the challenges of applying backtested strategies in live markets and the importance of accounting for **market microstructure** effects.

---

## Repository Contents

- `macaron_strategy.ipynb` – Jupyter notebook with code and analysis for the macaron strategy
- `README.md` – This file

---

## Disclaimer

This repository reflects **my individual contributions** to Team Jain Street’s participation in the 2025 IMC Prosperity Trading Challenge. All analysis and code are for educational and illustrative purposes only.
