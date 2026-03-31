<img width="1782" height="1924" alt="1dun_inr" src="https://github.com/user-attachments/assets/2d20ee91-029c-4a87-a60d-e633c7f0c0c5" />

### Fig. 1: Qualitative comparison against the interpolation method on the ICVL scene nachal_0823-1144. The upper panel displays the spectral density curves for the red-boxed region. The lower panel presents the reference RGB image, the 2D measurement, and a comparison of spectral slices: the first two rows show continuous spectral reconstruction on training wavelengths, while the last two rows demonstrate spectral super-resolution on rendering wavelengths.

### Tab. 1: Quantitative evaluation of continuous spectral reconstruction and spectral super-resolution across ten scenes from the ICVL dataset and the overall average. Each cell reports SAM (top), PSNR in dB (middle), and SSIM (bottom). To validate the superiority of our continuous design, we compare our Phy-CoSF against its discrete counterpart utilizing sophisticated interpolation under both 20 and 143 spectral bands settings. Best results are highlighted in **bold**.

| Methods | Scene 1 | Scene 2 | Scene 3 | Scene 4 | Scene 5 | Scene 6 | Scene 7 | Scene 8 | Scene 9 | Scene 10 | Avg |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Discrete + Interp. | 2.36<br>31.87<br>0.856 | 3.50<br>30.50<br>0.825 | 1.87<br>37.47<br>0.952 | 1.81<br>40.98<br>0.962 | 1.48<br>40.18<br>0.956 | 1.54<br>40.73<br>0.952 | 2.17<br>38.87<br>0.939 | 1.94<br>33.57<br>0.899 | 2.08<br>28.42<br>0.803 | 3.29<br>32.10<br>0.897 | 2.20<br>35.47<br>0.904 |
| **Phy-CoSF (Ours)** | **1.43**<br>**32.24**<br>**0.865** | **1.75**<br>**31.78**<br>**0.858** | **0.81**<br>**40.21**<br>**0.967** | **1.13**<br>**41.67**<br>**0.967** | **0.98**<br>**40.93**<br>**0.961** | **1.09**<br>**41.25**<br>**0.955** | **1.00**<br>**40.15**<br>**0.950** | **0.91**<br>**34.32**<br>**0.906** | **1.17**<br>**28.54**<br>**0.805** | **1.27**<br>**33.49**<br>**0.916** | **1.15**<br>**36.46**<br>**0.915** |

| Methods | Scene 1 | Scene 2 | Scene 3 | Scene 4 | Scene 5 | Scene 6 | Scene 7 | Scene 8 | Scene 9 | Scene 10 | Avg |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Discrete + Interp. | 2.43<br>31.85<br>0.856 | 3.52<br>30.47<br>0.824 | 2.00<br>37.41<br>0.951 | 1.84<br>40.95<br>0.962 | 1.50<br>40.16<br>0.956 | 1.59<br>40.71<br>0.951 | 2.26<br>38.74<br>0.938 | 2.09<br>33.50<br>0.899 | 2.19<br>28.39<br>0.803 | 3.42<br>32.01<br>0.897 | 2.28<br>35.42<br>0.904 |
| **Phy-CoSF (Ours)** | **1.39**<br>**32.25**<br>**0.865** | **1.70**<br>**31.76**<br>**0.857** | **0.82**<br>**40.21**<br>**0.967** | **1.12**<br>**41.66**<br>**0.967** | **0.97**<br>**40.92**<br>**0.961** | **1.08**<br>**41.25**<br>**0.955** | **1.00**<br>**40.09**<br>**0.949** | **0.90**<br>**34.32**<br>**0.905** | **1.15**<br>**28.55**<br>**0.805** | **1.26**<br>**33.47**<br>**0.916** | **1.14**<br>**36.45**<br>**0.915** |

-----

<img width="1491" height="1680" alt="1rgb" src="https://github.com/user-attachments/assets/25d79e1b-7b88-4a79-a18f-8044d45d5cec" />

### Fig. 2: Qualitative comparison against RGB super-resolution methods on simulated data. Top: RGB image, measurement, and spectral density curves (red box) for Scene 8, Bottom: Simulated discrete reconstruction results (2/28 channels).

-----

<img width="2412" height="1756" alt="2noise" src="https://github.com/user-attachments/assets/1fcf2aad-84c6-432d-9ef2-78836826a08e" />

### Fig. 3: Qualitative comparison under increasing noise levels on the ICVL scene BGU_0522-1217. The upper panel displays the spectral density curves for the red-boxed region. The lower panel presents the reference RGB image, the 2D measurement, and a comparison of spectral slices: the first row shows continuous spectral reconstruction on training wavelengths, while the last row demonstrates spectral super-resolution on rendering wavelengths.

-----

<img width="2199" height="1986" alt="3channel28" src="https://github.com/user-attachments/assets/0e7e68c8-1521-4030-8cdf-d293639fcd19" />

### Fig. 4: Qualitative comparison with other methods on 28 channels for the ICVL scene IDS_COLORCHECK_1020-1215-1. Due to time constraints, we compare our approach with the methods of Qin et al. and Wu et al. The upper panel displays the spectral density curves for the red-boxed region. The lower panel presents the reference RGB image, the 2D measurement, and a comparison of spectral slices: the first two rows show continuous spectral reconstruction on training wavelengths, while the last two rows demonstrate spectral super-resolution on rendering wavelengths.

-----

<img width="2030" height="1178" alt="3spectral-profile" src="https://github.com/user-attachments/assets/ece67ce8-c279-4f06-97e7-43cab5222d02" />

### Fig. 5: Spectral profile and band distribution analysis for the ICVL scene hill_0325-1242. The main plot displays the spectral density curve for the red-boxed region, illustrating the training samples (green dots) and unseen rendering targets (red crosses) against the ground truth profile. The bottom panel visualizes the continuous distribution of these spectral bands. Additionally, the right legend details the specific wavelength values for both the training bands and the unseen rendering bands.

-----

<img width="1400" height="1000" alt="4loss" src="https://github.com/user-attachments/assets/d2e919db-4a78-459e-a28b-02a990677e75" />

### Fig. 6: Convergence analysis of our Phy-CoSF over 200 epochs. The subplots display the training loss alongside testing metrics (PSNR, SSIM, and SAM). As observed, our method exhibits rapid and highly stable convergence without significant oscillations. The steady and monotonic improvement across all metrics highlights the robust learning capability and superior reconstruction performance of our continuous framework.

-----

<img width="2343" height="2039" alt="4mask" src="https://github.com/user-attachments/assets/27ac4e89-90c6-4077-9b10-7cea3c12b222" />

### Fig. 7: Qualitative comparison using a noise-injected mask on the ICVL scene IDS_COLORCHECK_1020-1215-1. The upper panel displays the spectral density curves for the red-boxed region. The lower panel presents the reference RGB image, the 2D measurement, and a comparison of spectral slices: the first two rows show continuous spectral reconstruction on training wavelengths, while the last two rows demonstrate spectral super-resolution on rendering wavelengths.

-----
