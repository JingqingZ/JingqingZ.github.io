---
title: "Short Term Traffic Flow Prediction with Spatial-Temporal Neural Networks on England Highway"
collection: projects
type: "Projects"
permalink: /projects/2017-09-EnglandHighway
date: 2017-09-15
location: "London, UK"
avatar: "https://jingqingz.github.io/files/projects/2017-09-EnglandHighway/avatar.png"
---

This project is initially submitted in partial fulfillment 
of the requirements for the MRes degree in Advanced Computing 
of Imperial College London. Accepted as a poster in [MLImperial2017](http://www.imperial.ac.uk/machine-learning/).


## Abstract 

Both temporal and spatial features provide significant implications for short-term
traffic volume prediction. The problem is challenging due to various non-linear temporal
dynamics at different locations, complicated spatial dependencies and difficulty
for longer-step ahead forecasting. We propose two deep learning models, CNNLSTM
with attention mechanism (CNN-LSTM-Attn) and Temporal-Spatial-LSTM (TSLSTM)
to incorporate temporal and spatial correlations. Experiments show that both
models outperform baselines on the Highways England dataset and the CNN-LSTMAttn
achieves lowest MAPE 9.26% on 2-hour traffic volume prediction. We also
evaluate the CNN-LSTM-Attn on the KDDCUP17 dataset and our model defeats the
model that got first place in the competition with lower MAPE 10.48%. Our models
achieve 2-hour forecasting, which is longer than previous literature, with outstanding
accuracy and robustness.


## Demo

England Highway Prediction Visualisation (GIF)
<div>
    <img src="https://jingqingz.github.io/files/projects/2017-09-EnglandHighway/demo.gif" style="width: 80%;"/>
</div>

<br/>
Visulisation on Global Data Observatory
<div>
    <img src="https://jingqingz.github.io/files/projects/2017-09-EnglandHighway/gdo_pano.png" style="width: 80%;"/>
</div>

## Files

[Poster](https://jingqingz.github.io/files/projects/2017-09-EnglandHighway/poster.pdf) 
[Thesis](https://jingqingz.github.io/files/projects/2017-09-EnglandHighway/report.pdf) 


