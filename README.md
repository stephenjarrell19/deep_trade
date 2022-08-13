# Deep Trade

A home for all trading analytics, POC agents, indicator generators, supervised modeling, and reinforcement learning / policy learning.

##  Motivation

Develop a bot that does not trade for breakouts, but trades to minimize risk and optimize for R-values.

## Proof of Concept 

Create a very accurate neural network for identifying ONLY support and resistance levels. If you can draw a border that can identify the box of support and resistance on any given stock (based on its historical data) consistently, then match that across different time frames, with a high degree of accuracy, then optimize for Risk to Reward values (R).
## Implementation ideas
### SnR Charter
Trying to create a NN that can look at a chart over multiple time frames, and it needs to be able to: 
  1. Draw support and resistance areas
  2. Interpolate over time (matching or correlating support levels to make support patterns more salient)
 
 If 1 and 5 min support lines correlate, then its more salient.
 ### Broker
 
Trained on Human_trader strategy, using "When x happens, you can buy and sell at y."
 interfaces with SnR charter and _____(other input streams) to decide to take setup or not.

**Use R-values as optimization metrics.**

## Resources
Transformer-Based Capsule Network For Stock Movements Prediction: https://aclanthology.org/W19-5511.pdf
QuantConnect (real-time data): https://www.quantconnect.com/?gclid=CjwKCAjw9NeXBhAMEiwAbaY4lis7p7lLTI_tgP8ZRj7LFL9nO84oagiMFyPmuoHcSyzrmt_SxoxDJRoCwdkQAvD_BwE

How to Day Trade youtube playlist: https://www.youtube.com/playlist?list=PLBQ51w5jhEqVx9r9siB3GgB9YKj-KaKLP



### Models



### 
