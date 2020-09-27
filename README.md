# OSIC Pulmonary Fibrosis Progression Competition from Kaggle

The challenge is to predict a patient's severity of decline in lung function based on a CT scan of their lungs, output from a spirometer, which measures the volume of air inhaled and exhaled. The machine learning model will use the image, metadata, and baseline FVC as input.
This competition is evaluated on a modified version of the Laplace Log Likelihood. The metric is designed to reflect both the accuracy and certainty of each prediction.

```math
\sigma_{clipped} = \max(\sigma,70),
\Delta = \min\(\|FVC_{true} - FVC_{predicted}\|, 1000\),
metric = -\frac{\sqrt(2)\Delta}{\sigma_{clipped}} - \ln\(\sqrt(2) \sigma_{clipped}\).
```

