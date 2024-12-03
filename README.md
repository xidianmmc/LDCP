# LDCP
Implemetation of Adaptive Chroma Prediction Based on Luma Difference for H.266/VVC

Abstract— Cross-component chroma prediction plays an
important role in improving coding efffciency for H.266/VVC.
We use the differences between reference samples and the
predicted sample to design an attention model for chroma
prediction, namely luma difference-based chroma prediction
(LDCP). Speciffcally, the luma differences (LDs) between reference
 samples and the predicted sample are employed as the
input of the attention model, which is designed as a softmax
function to map LDs to chroma weights nonlinearly. Finally,
a weighted chroma prediction is conducted based on the weights
and chroma reference samples. To provide adaptive weights, the
model parameter of the softmax function can be determined
based on the template (T-LDCP) or offfine learning (L-LDCP),
respectively. Experimental results show that the T-LDCP achieves
BD-rate reductions of 0.34%, 2.02%, and 2.34% for the Y, Cb,
and Cr components, and the L-LDCP brings 0.32%, 2.06%, and
2.21% BD-rate savings for Y, Cb, and Cr components, respectively.
 The L-LDCP introduces slight encoding and decoding time
increments, i.e., 2% and 1%, when integrated into the latest VVC
test model version 18.0. Besides, the LDCP can be implemented
by a pixel-level parallelization which is hardware-friendly.
