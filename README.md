# AlgoSoc-Sessions

Master: ![Master](https://travis-ci.com/Joearrowsmith/AlgoSoc-Sessions.svg?branch=master)

### agent_0_echo.py 
- The simplest possible agent: prints the current bid, ask and time. Works for backtest and real-time data.

### agent_1_simple_macd.py
- A simple momentum strategy looking at the cross over of two moving averages.

### agent_2_simple_risk_managed_macd.py
- A momentum strategy with some risk measures. Inherits the base rules from simple MACD and implements a static stop loss and take profit on top.

### agent_3_risk_managed_macd.py
- A momentum strategy with some risk measures. Inherits the base rules from simple MACD and implements a dynamic stop loss if the asset becomes too volatile.

### build_dataset.py
- A function to collect your own data using the live datastream from the pedlar server.

### param_optimisation.py
- A function to determine the expected return from using an agents different parameters.

### test_agents.py
- A script to test the code builds when uploaded to github.

---

## Best Agent Backtest Performance through Versions:

1. Simple MACD \[fast length (fl): 20, slow length (sl): 40\] 
   - returns = -2.98...
2. Simple MACD with "optimal" lengths \[fl: 120, sl: 250\]
   - returns = 0.099...
3. MACD with "optimal" length and dynamic risk control \[fl: 120, sl: 250, ret length (rl): 100, risk scaling factor (rsf): 3.5\]
   - returns = 0.899...
4. MACD with "optimal" length and dynamic risk control \[fl : 120, sl : 250, stop loss scaling (sls)} : 1.1, take profit scaling (tps) : 3.5]
   - returns = 1.909...

---

## Next Steps:

### For agents:
1. Decision tree based agent
2. Linear model based agent
3. NN based agent
4. RNN based agent
5. RL based agent

### For finding parameters:
1. Grid search
2. Random search
3. Gradient-based search

### Combining multiple signals & agents:
1. Ensemble of agents
2. K-Armed bandits

### Risk Control:
1. Time dependent behaviour (e.g. varying behaviour around market open/close)
2. Real time statistics
3. Add post-analysis of trades made.

---

<img src="misc/icats_logo.png" alt="icats_logo" width="150"/>

# About us:

### [Algo soc website](http://www.algosoc.com)

### [Algo soc slack](https://algosoc.slack.com)

## Our trading platform Pedlar:

[Imperial pedlar server](http://icats.doc.ic.ac.uk) &rightarrow; (requires access to Imperial Wifi Network)

![Pedlar](misc/pedlarweb_screenshot.jpg)

#### You can contact us at: <algo.trade@imperial.ac.uk>

<img src="misc/icats_logo.png" alt="icats_logo" width="150"/>