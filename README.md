
rQuarto project link: https://patrick-lefler.github.io/Bitcoin-Halving-Visualization-PythonQuarto/

### Summary

A quantitative analysis and visualization of Bitcoin's supply schedule, demonstrating the asymptotic approach to the 21 million supply cap through programmatic halvings

### Project Overview

This project utilizes Python within a Quarto framework to model Bitcoin's monetary policy. By simulating the block reward reduction that occurs every 210,000 blocks, this notebook generates interactive visualizations of the geometric series that defines Bitcoin's scarcity.The analysis projects approximately 34 halving events, calculating supply metrics from the genesis block in 2009 through the theoretical depletion of block rewards in 2140

### Visualizations

The project generates four key outputs:
1. Cumulative Supply Curve: A linear-scale visualization of the total Bitcoin supply over time, showing the asymptotic approach to the 21,000,000 cap.
2. Remaining Supply Decay: A log-scale analysis of the unmined Bitcoin remaining, highlighting the consistent exponential decay of available supply
3. Block Reward Schedule: A bar chart tracking the reduction of block rewards from 50 BTC down to effectively zero5.Halving
4. Data Table: A detailed tabular view of specific halving epochs, calculating the exact BTC mined per period and the percentage of the cap reached
  
### Technical Stack Framework: 
* Quarto (v1.2+)
* Language: Python
* Key Libraries: pandas & numpy
* Data generation and manipulation: plotly:
* Interactive graphing (Log scales, hover templates)

### Methodology
The core logic relies on a simulation function generate_halving_data() which iterates through 34 projected halving events10. 

### The Mathematical Model
The total supply is calculated as a geometric series
$$\text{Total Supply} = \sum_{n=0}^{64} 210{,}000 \times \frac{50}{2^n}$$

* Parameters used:Initial Block Reward: 50 BTCHalving 
* Interval: 210,000 blocks (~4 years)
* Termination Criteria: When block reward < 1 Satoshi ($10^{-8}$ BTC)12

### Project Structure
├── Bitcoin_Halving_V1.2.qmd  # Main Quarto source file
├── README.md                 # Project documentation
└── [Generated HTML]          # Output file (after rendering)

### License
This project is open-source. Feel free to fork and modify the simulation parameters to test different supply curve scenarios.
