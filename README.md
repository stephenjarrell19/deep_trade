# Deep Trade

A home for all trading analytics, POC agents, indicator generators, supervised modeling, and reinforcement learning / policy learning.

##  Proof Of Concept

Develop a bot that can **identify support and resistance levels** and optimize R-values. 

![display_text](https://user-images.githubusercontent.com/49171243/184468830-276380a0-9767-4185-a56b-460a0a16c6ac.jpg)

### Customizable to Risk Tolerance
The goal is not to develop a model that trades for breakout wins, but instead a model that trades on support and resistance trends, buying at support and selling in any margin between the buying price and resistance. The margin is an area, and the selling price within that margin can be decided based upon some quantity of acceptable risk. A high risk tolerance could attempt to maximize positive R-values, while a lower risk tolerance agent would simply take home the easy profit (small R-values).

### What are R-values?
https://smartforexlearning.com/risk-r-and-r-multiples-explained/

## Implementation Brainstorming

Create a very accurate neural network for identifying ONLY support and resistance levels. If you can draw a border that can identify the box of support and resistance on any given stock (based on its historical data) consistently, then match that across different time frames, with a high degree of accuracy, then optimize for Risk to Reward values (R).

### SnR Charter
Trying to create a NN that can look at a chart over multiple time frames, and it needs to be able to: 
  1. Draw support and resistance areas
  2. Interpolate over time (matching or correlating support levels to make support patterns more salient)
 
 If 1 and 5 min support lines correlate, then its more salient.
 ### Broker
 
Trained on Human_trader strategy, using "When x happens, you can buy and sell at y."
 interfaces with SnR charter and _____(other input streams) to decide to take setup or not.

**Use R-values as optimization metrics.**

## Data Needs
- Order Flow
- Open, Close, High, Low

## Resources
### Core
R-Values Explained: https://smartforexlearning.com/risk-r-and-r-multiples-explained/
### Misc
WaveNet Time Series Prediction: https://arxiv.org/pdf/1609.03499.pdf
Transformer-Based Capsule Network For Stock Movements Prediction: https://aclanthology.org/W19-5511.pdf
QuantConnect (real-time data): https://www.quantconnect.com/?gclid=CjwKCAjw9NeXBhAMEiwAbaY4lis7p7lLTI_tgP8ZRj7LFL9nO84oagiMFyPmuoHcSyzrmt_SxoxDJRoCwdkQAvD_BwE
How to Day Trade youtube playlist: https://www.youtube.com/playlist?list=PLBQ51w5jhEqVx9r9siB3GgB9YKj-KaKLP

### Models
WaveNet Time Series Prediction: https://arxiv.org/pdf/1609.03499.pdf


### 
