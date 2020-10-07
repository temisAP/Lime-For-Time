# LIME For Time

We applied the LIME algorithm (LIME - Local Interpretable Model-Agnostic Explanations) developed by Marco Tulio Ribeiro, Sameer Singh and Carlos Guestrin  ([paper](https://arxiv.org/pdf/1602.04938.pdf), [GitHub](https://github.com/marcotcr/lime)) to time series classification. 

LIME is used to better understand prediction made by complex black-box ML models. By making use of a transparent, interpretable model the algorithm tries to approximate the black-box locally in vicinty of a specific data sample.

A given example instance is perturbed (i.e. parts of its features are 'switched off', pixels greyed out for example) many times and fed to the black-box. The approximating model then learns which features have the most influence on the final prediction.

The LIME package only supports image, text and tabular data. We extended it to be able to deal with time series data.

![Results on the coffee dataset](/demo/results/coffee/coffee_24_10_noise.JPG)

![Results on the ecg dataset](/demo/results/ecg/ecg_17_5_total_mean.JPG)
