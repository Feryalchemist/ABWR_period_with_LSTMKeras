#Data Driven Reactor Stability Forecasting Using Long Short-Term Memory on Recurent Neural Network

---
This is personal project on Keras/LSTM, in which I've done several years ago.

The goal of this program is to predict the reactor stability by neural network and data driven method. Since the neutron flux over time shouldn't be increase dramatically by order of exp the Reactor Period should be kept at near infinite number (in the case of this simulation max.measurement.value=9999)

The Transient Reactor Parameter is taken by simulating the reactor operation with PcTran ABWR Simulator (http://www.microsimtech.com/abwr/). Data obtained by a single simulation of an initial condition. Data provided in  time series multivariate datasets with 91 features and 301 timesteps. 

LSTM was chosen because of its robustness in handling recurring data and predicting certain result from many features. To summon the LSTM module, keras API should be used. Keras is an API for deep learning problem solving (https://keras.io).

##*Update*:

*This solution to search the best prediction model is unavailable due to non-convergent input. This problem caused by Sklearn.Preprocessing.Scaler was failed to scale the fitted data. Thera are still so many scaled features value with >1 variance.* 

*Further data preprocessing such as target value shifting and re-evaluation of lookback method should be revised*
