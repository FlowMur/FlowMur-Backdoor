# FlowMur-Rebuttal

## C1: Auxiliary dataset size (205A, 205B, 205D)
<img src="./img/data-balance.png" width="75%">

## C2: Additional datasets with long sample duration (205A, 205B, 205C)
<img src="./img/fsc.png" width="60%">

## C3: Additional defense (205B, 205C)
### 1. Defense performance of filters on FlowMur
<img src="./img/defense.png" width="50%">

### 2. Defense performance of Beatrix on FlowMur
* [Ma et al.](https://www.ndss-symposium.org/wp-content/uploads/2023/02/ndss2023_s69_paper.pdf) observed that although the infected model identifies both clean samples of the target class and poisonous samples as the target class, these two sets of samples are disjoint in the pixel space. Therefore, the intermediate representations of the poisonous samples differ from those of the clean samples. Based on this observation, [Ma et al.](https://www.ndss-symposium.org/wp-content/uploads/2023/02/ndss2023_s69_paper.pdf) proposed Beatrix, a defense method that leverages Gram Matrices to model the intermediate representations of samples, enabling the discrimination between benign and poisonous samples. Additionally, it further employs kernel-based testing to identify the infected label (i.e., the target class). Figure 14 demonstrates the defense performance of Beatrix on FlowMur and baselines. As shown in Figure 14, it is evident that the anomaly index of the infected label exceeds the predefined threshold on FKD for all three attack methods, indicating the effectiveness of Beatrix in defending against these attacks. From Fig. 14 we can see that the anomaly index of the infected label for all three attack methods are greater than the predefined threshold on FKD, indicating that Beatrix is effective for defending against all three attacks on FCK. However, for SCD, it becomes apparent that the anomaly index of the infected label in the case of FlowMur falls below the threshold, indicating Beatrix's inability to defend against FlowMur in the context of SCD.
<img src="./img/Beatrix.png" width="50%">

## 205A_Response
<img src="./img/small-cnn.png" width="55%">
<img src="./img/large-cnn.png" width="48%">
<img src="./img/rnn.png" width="31%">
<img src="./img/resnet.png" width="65%">

## 205B_Response
### 1. *p*-values
<img src="./img/fsc.png" width="60%">

### 2. Tests on speaker recognition
<img src="./img/speaker.png" width="40%">

### 3. SNR
<img src="./img/SNR.png" width="50%">

## 205C_Response
<img src="./img/fig7.png" width="50%">

## 205D_Response
### 1. Extended Table 1
<img src="./img/table1.png" width="100%">

### 2. Audio waveforms, spectrograms and MFCCs for different cases 
<img src="./img/sample-fig.png" width="100%">

### 3. An attack example of FlowMur 
<img src="./img/backdoor-inference.png" width="52%">

### 4. Experimental settings and datasets statistics
<img src="./img/setting-1.png" width="29%">
<img src="./img/setting-2.png" width="35%">
<img src="./img/setting-3.png" width="35%">
<img src="./img/setting4.png" width="60%">
