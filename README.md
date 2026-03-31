<img width="1782" height="1924" alt="1dun_inr" src="https://github.com/user-attachments/assets/2d20ee91-029c-4a87-a60d-e633c7f0c0c5" />

### Fig. 1: Qualitative comparison against the interpolation method on the ICVL scene nachal_0823-1144. The upper panel displays the spectral density curves for the red-boxed region. The lower panel presents the reference RGB image, the 2D measurement, and a comparison of spectral slices: the first two rows show continuous spectral reconstruction on training wavelengths, while the last two rows demonstrate spectral super-resolution on rendering wavelengths.

### Tab. 1: Quantitative evaluation of continuous spectral reconstruction and spectral super-resolution across ten scenes from the ICVL dataset and the overall average. Each cell reports SAM (top), PSNR in dB (middle), and SSIM (bottom). To validate the superiority of our continuous design, we compare our Phy-CoSF against its discrete counterpart utilizing sophisticated interpolation under both 143 and 20 spectral bands settings. Best results are highlighted in **bold**.

| Continuous Reconstruction | Scene 1 | Scene 2 | Scene 3 | Scene 4 | Scene 5 | Scene 6 | Scene 7 | Scene 8 | Scene 9 | Scene 10 | Avg |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Interpolation | 2.43<br>31.85<br>0.856 | 3.52<br>30.47<br>0.824 | 2.00<br>37.41<br>0.951 | 1.84<br>40.95<br>0.962 | 1.50<br>40.16<br>0.956 | 1.59<br>40.71<br>0.951 | 2.26<br>38.74<br>0.938 | 2.09<br>33.50<br>0.899 | 2.19<br>28.39<br>0.803 | 3.42<br>32.01<br>0.897 | 2.28<br>35.42<br>0.904 |
| **Phy-CoSF(Ours)** | **1.39**<br>**32.25**<br>**0.865** | **1.70**<br>**31.76**<br>**0.857** | **0.82**<br>**40.21**<br>**0.967** | **1.12**<br>**41.66**<br>**0.967** | **0.97**<br>**40.92**<br>**0.961** | **1.08**<br>**41.25**<br>**0.955** | **1.00**<br>**40.09**<br>**0.949** | **0.90**<br>**34.32**<br>**0.905** | **1.15**<br>**28.55**<br>**0.805** | **1.26**<br>**33.47**<br>**0.916** | **1.14**<br>**36.45**<br>**0.915** |

| Super-Resolution | Scene 1 | Scene 2 | Scene 3 | Scene 4 | Scene 5 | Scene 6 | Scene 7 | Scene 8 | Scene 9 | Scene 10 | Avg |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Interpolation | 2.36<br>31.87<br>0.856 | 3.50<br>30.50<br>0.825 | 1.87<br>37.47<br>0.952 | 1.81<br>40.98<br>0.962 | 1.48<br>40.18<br>0.956 | 1.54<br>40.73<br>0.952 | 2.17<br>38.87<br>0.939 | 1.94<br>33.57<br>0.899 | 2.08<br>28.42<br>0.803 | 3.29<br>32.10<br>0.897 | 2.20<br>35.47<br>0.904 |
| **Phy-CoSF(Ours)** | **1.43**<br>**32.24**<br>**0.865** | **1.75**<br>**31.78**<br>**0.858** | **0.81**<br>**40.21**<br>**0.967** | **1.13**<br>**41.67**<br>**0.967** | **0.98**<br>**40.93**<br>**0.961** | **1.09**<br>**41.25**<br>**0.955** | **1.00**<br>**40.15**<br>**0.950** | **0.91**<br>**34.32**<br>**0.906** | **1.17**<br>**28.54**<br>**0.805** | **1.27**<br>**33.49**<br>**0.916** | **1.15**<br>**36.46**<br>**0.915** |

-----

<img width="1491" height="1680" alt="1rgb" src="https://github.com/user-attachments/assets/25d79e1b-7b88-4a79-a18f-8044d45d5cec" />

### Fig. 2: Qualitative comparison against RGB super-resolution methods on simulated data. Top: RGB image, measurement, and spectral density curves (red box) for Scene 8, Bottom: Simulated discrete reconstruction results (2/28 channels).

### Tab. 2: Quantitative comparison against RGB super-resolution baselines on simulated data. The average PSNR and SSIM metrics are reported. Best results are highlighted in **bold**.

| Methods | PSNR (dB) | SSIM |
| :--- | :---: | :---: |
| SSRMamba | 35.21 | 0.915 |
| SSRNet | 35.55 | 0.918 |
| **Phy-CoSF(Ours)** | **39.80** | **0.978** |

-----

<img width="2412" height="1756" alt="2noise" src="https://github.com/user-attachments/assets/1fcf2aad-84c6-432d-9ef2-78836826a08e" />

### Fig. 3: Qualitative comparison under increasing noise levels on the ICVL scene BGU_0522-1217. The upper panel displays the spectral density curves for the red-boxed region. The lower panel presents the reference RGB image, the 2D measurement, and a comparison of spectral slices: the first row shows continuous spectral reconstruction on training wavelengths, while the last row demonstrates spectral super-resolution on rendering wavelengths.

### Tab. 3: Noise robustness analysis of our Phy-CoSF across different settings. We simulate physical measurement noise by adding Gaussian noise at levels of 10, 20, and 30. The top sub-table shows the performance for continuous spectral reconstruction (143 bands), while the bottom sub-table presents the results for spectral super-resolution (20 bands). Metrics reported are SAM, PSNR (dB), and SSIM (top to bottom in each cell).

| Continuous Reconstruction | Scene 1 | Scene 2 | Scene 3 | Scene 4 | Scene 5 | Scene 6 | Scene 7 | Scene 8 | Scene 9 | Scene 10 | Avg |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Noise Level = 0 | 3.57<br>31.32<br>0.821 | 4.00<br>30.86<br>0.812 | 3.02<br>36.59<br>0.910 | 3.99<br>38.29<br>0.924 | 3.60<br>38.27<br>0.928 | 3.96<br>38.61<br>0.920 | 3.68<br>36.88<br>0.900 | 2.46<br>33.18<br>0.860 | 2.62<br>28.15<br>0.763 | 2.86<br>32.41<br>0.871 | 3.37<br>34.46<br>0.871 |
| Noise Level = 10 | 5.04<br>30.13<br>0.762 | 5.59<br>29.76<br>0.756 | 4.76<br>33.81<br>0.832 | 5.87<br>35.89<br>0.874 | 5.31<br>36.41<br>0.891 | 5.82<br>36.61<br>0.879 | 5.43<br>34.69<br>0.842 | 3.73<br>31.62<br>0.792 | 3.82<br>27.49<br>0.705 | 4.18<br>31.02<br>0.800 | 4.95<br>32.74<br>0.813 |
| Noise Level = 20 | 6.29<br>29.16<br>0.709 | 6.89<br>28.89<br>0.706 | 6.20<br>31.99<br>0.755 | 7.33<br>34.25<br>0.828 | 6.79<br>34.80<br>0.852 | 7.33<br>34.94<br>0.838 | 6.87<br>33.14<br>0.788 | 4.87<br>30.28<br>0.721 | 4.93<br>26.79<br>0.645 | 5.42<br>29.78<br>0.723 | 6.29<br>31.40<br>0.757 |

| Super-Resolution | Scene 1 | Scene 2 | Scene 3 | Scene 4 | Scene 5 | Scene 6 | Scene 7 | Scene 8 | Scene 9 | Scene 10 | Avg |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Noise Level = 0 | 3.67<br>31.26<br>0.819 | 4.13<br>30.84<br>0.810 | 3.13<br>36.44<br>0.906 | 4.12<br>38.16<br>0.922 | 3.73<br>38.12<br>0.926 | 4.07<br>38.49<br>0.918 | 3.78<br>36.80<br>0.898 | 2.56<br>33.09<br>0.857 | 2.70<br>28.13<br>0.761 | 2.92<br>32.38<br>0.869 | 3.48<br>34.37<br>0.869 |
| Noise Level = 10 | 5.20<br>30.02<br>0.759 | 5.80<br>29.69<br>0.753 | 4.93<br>33.62<br>0.826 | 6.05<br>35.72<br>0.870 | 5.50<br>36.24<br>0.887 | 6.02<br>36.40<br>0.876 | 5.60<br>34.55<br>0.838 | 3.85<br>31.46<br>0.787 | 3.93<br>27.42<br>0.701 | 4.32<br>30.93<br>0.796 | 5.12<br>32.61<br>0.809 |
| Noise Level = 20 | 6.54<br>29.03<br>0.704 | 7.13<br>28.82<br>0.703 | 6.47<br>31.71<br>0.747 | 7.58<br>34.06<br>0.824 | 7.06<br>34.56<br>0.846 | 7.51<br>34.81<br>0.836 | 7.10<br>32.93<br>0.782 | 5.05<br>30.08<br>0.714 | 5.16<br>26.67<br>0.639 | 5.64<br>29.58<br>0.716 | 6.52<br>31.22<br>0.751 |

-----

<img width="2199" height="1986" alt="3channel28" src="https://github.com/user-attachments/assets/0e7e68c8-1521-4030-8cdf-d293639fcd19" />

### Fig. 4: Qualitative comparison with other methods on 28 channels for the ICVL scene IDS_COLORCHECK_1020-1215-1. Due to time constraints, we compare our approach with the methods of Qin et al. and Wu et al. The upper panel displays the spectral density curves for the red-boxed region. The lower panel presents the reference RGB image, the 2D measurement, and a comparison of spectral slices: the first two rows show continuous spectral reconstruction on training wavelengths, while the last two rows demonstrate spectral super-resolution on rendering wavelengths.

### Tab. 4: Quantitative evaluation against recent state-of-the-art architectures (Qin et al. and Wu et al).  The top sub-table shows results for continuous spectral reconstruction (143 bands), while the bottom sub-table shows spectral super-resolution (20 bands). Note that our Phy-CoSF achieves the lowest overall SAM and highly competitive spatial fidelity.

| Continuous Reconstruction | Scene 1 | Scene 2 | Scene 3 | Scene 4 | Scene 5 | Scene 6 | Scene 7 | Scene 8 | Scene 9 | Scene 10 | Avg |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Mijun-5stg | 2.08<br>**32.60**<br>**0.873** | 2.68<br>31.57<br>0.855 | 1.49<br>39.33<br>0.962 | 1.65<br>**42.08**<br>**0.970** | 1.41<br>40.99<br>0.961 | 1.49<br>41.03<br>0.954 | 1.67<br>39.62<br>0.945 | 1.58<br>34.26<br>**0.908** | 1.91<br>**28.45**<br>**0.810** | 2.24<br>33.13<br>0.906 | 1.82<br>36.31<br>0.914 |
| Lade-DUN-5stg | 2.12<br>32.44<br>0.870 | 2.67<br>31.56<br>0.857 | 1.42<br>39.39<br>0.963 | 1.66<br>41.93<br>0.969 | 1.34<br>**41.30**<br>**0.962** | 1.52<br>**41.21**<br>**0.955** | 1.65<br>39.42<br>0.944 | 1.60<br>34.09<br>0.906 | 1.88<br>28.02<br>0.806 | 2.17<br>**33.38**<br>0.909 | 1.80<br>36.27<br>0.914 |
| **Phy-CoSF-5stg (Ours)** | **1.37**<br>32.32<br>0.866 | **1.66**<br>**31.78**<br>**0.859** | **0.80**<br>**39.94**<br>**0.965** | **1.14**<br>41.38<br>0.965 | **0.98**<br>40.89<br>0.960 | **1.10**<br>41.14<br>0.954 | **0.99**<br>**40.46**<br>**0.952** | **0.89**<br>**34.31**<br>0.906 | **1.14**<br>28.30<br>0.805 | **1.27**<br>33.28<br>**0.913** | **1.13**<br>**36.38**<br>**0.915** |

| Super-Resolution | Scene 1 | Scene 2 | Scene 3 | Scene 4 | Scene 5 | Scene 6 | Scene 7 | Scene 8 | Scene 9 | Scene 10 | Avg |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Mijun-5stg | 2.11<br>32.59<br>**0.873** | 2.70<br>31.59<br>0.856 | 1.52<br>39.31<br>0.963 | 1.65<br>**42.08**<br>**0.970** | 1.39<br>41.00<br>0.961 | 1.47<br>41.04<br>0.954 | 1.69<br>39.64<br>0.945 | 1.59<br>34.24<br>**0.908** | 1.94<br>**28.44**<br>**0.810** | 2.24<br>33.14<br>0.906 | 1.83<br>36.31<br>**0.915** |
| Lade-DUN-5stg | 2.17<br>32.42<br>0.870 | 2.70<br>31.58<br>0.858 | 1.45<br>39.36<br>0.963 | 1.67<br>41.93<br>0.969 | 1.34<br>**41.29**<br>**0.962** | 1.51<br>**41.20**<br>**0.955** | 1.66<br>39.47<br>0.945 | 1.62<br>34.06<br>0.906 | 1.92<br>27.99<br>0.806 | 2.19<br>**33.38**<br>0.910 | 1.82<br>36.27<br>0.914 |
| **Phy-CoSF-5stg (Ours)** | **1.40**<br>32.32<br>0.867 | **1.69**<br>**31.80**<br>**0.859** | **0.80**<br>**39.94**<br>**0.965** | **1.15**<br>41.39<br>0.965 | **0.99**<br>40.89<br>0.960 | **1.11**<br>41.14<br>0.954 | **0.99**<br>**40.51**<br>**0.952** | **0.90**<br>**34.31**<br>0.905 | **1.16**<br>28.30<br>0.804 | **1.29**<br>33.30<br>**0.914** | **1.15**<br>**36.39**<br>**0.915** |

-----

<img width="2030" height="1178" alt="3spectral-profile" src="https://github.com/user-attachments/assets/ece67ce8-c279-4f06-97e7-43cab5222d02" />

### Fig. 5: Spectral profile and band distribution analysis for the ICVL scene hill_0325-1242. The main plot displays the spectral density curve for the red-boxed region, illustrating the training samples (green dots) and unseen rendering targets (red crosses) against the ground truth profile. The bottom panel visualizes the continuous distribution of these spectral bands. Additionally, the right legend details the specific wavelength values for both the training bands and the unseen rendering bands.

-----

<img width="1400" height="1000" alt="4loss" src="https://github.com/user-attachments/assets/d2e919db-4a78-459e-a28b-02a990677e75" />

### Fig. 6: Convergence analysis of our Phy-CoSF over 200 epochs. The subplots display the training loss alongside testing metrics (PSNR, SSIM, and SAM). As observed, our method exhibits rapid and highly stable convergence without significant oscillations. The steady and monotonic improvement across all metrics highlights the robust learning capability and superior reconstruction performance of our continuous framework.

-----

<img width="2343" height="2039" alt="4mask" src="https://github.com/user-attachments/assets/27ac4e89-90c6-4077-9b10-7cea3c12b222" />

### Fig. 7: Qualitative comparison using a noise-injected mask on the ICVL scene IDS_COLORCHECK_1020-1215-1. The upper panel displays the spectral density curves for the red-boxed region. The lower panel presents the reference RGB image, the 2D measurement, and a comparison of spectral slices: the first two rows show continuous spectral reconstruction on training wavelengths, while the last two rows demonstrate spectral super-resolution on rendering wavelengths.

### Tab. 5: Quantitative comparison between the noise-injected mask and the original training mask on the ICVL dataset. The upper sub-table presents the results for continuous spectral reconstruction (143 bands). The lower sub-table demonstrates spectral super-resolution (20 bands). Metrics reported in each cell are SAM (top), PSNR in dB (middle), and SSIM (bottom).

| Continuous Reconstruction | Scene 1 | Scene 2 | Scene 3 | Scene 4 | Scene 5 | Scene 6 | Scene 7 | Scene 8 | Scene 9 | Scene 10 | Avg |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| w/ Noise Mask | 1.41<br>32.18<br>0.864 | 1.72<br>31.76<br>**0.857** | 0.83<br>40.13<br>0.966 | 1.13<br>41.61<br>0.967 | 0.98<br>**40.93**<br>0.961 | 1.09<br>41.22<br>**0.955** | 1.01<br>40.03<br>0.949 | 0.90<br>34.24<br>0.904 | 1.16<br>28.52<br>0.804 | 1.27<br>**33.48**<br>0.916 | 1.15<br>36.41<br>0.914 |
| **Phy-CoSF-9stg (Ours)** | **1.39**<br>**32.25**<br>**0.865** | **1.70**<br>**31.76**<br>0.857 | **0.82**<br>**40.21**<br>**0.967** | **1.12**<br>**41.66**<br>**0.967** | **0.97**<br>40.92<br>**0.961** | **1.08**<br>**41.25**<br>0.955 | **1.00**<br>**40.09**<br>**0.949** | **0.90**<br>**34.32**<br>**0.905** | **1.15**<br>**28.55**<br>**0.805** | **1.26**<br>33.47<br>**0.916** | **1.14**<br>**36.45**<br>**0.915** |

| Super-Resolution | Scene 1 | Scene 2 | Scene 3 | Scene 4 | Scene 5 | Scene 6 | Scene 7 | Scene 8 | Scene 9 | Scene 10 | Avg |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| w/ Noise Mask | 1.45<br>32.17<br>0.864 | 1.78<br>31.78<br>0.858 | 0.83<br>40.13<br>0.966 | 1.14<br>41.62<br>0.967 | 0.98<br>**40.93**<br>**0.961** | 1.10<br>41.21<br>**0.956** | 1.01<br>40.08<br>0.949 | 0.92<br>34.24<br>0.905 | 1.18<br>28.51<br>0.804 | 1.28<br>**33.50**<br>0.916 | 1.17<br>36.42<br>0.915 |
| **Phy-CoSF-9stg (Ours)** | **1.43**<br>**32.24**<br>**0.865** | **1.75**<br>**31.78**<br>**0.858** | **0.81**<br>**40.21**<br>**0.967** | **1.13**<br>**41.67**<br>**0.967** | **0.98**<br>40.93<br>**0.961** | **1.09**<br>**41.25**<br>0.955 | **1.00**<br>**40.15**<br>**0.950** | **0.91**<br>**34.32**<br>**0.906** | **1.17**<br>**28.54**<br>**0.805** | **1.27**<br>33.49<br>**0.916** | **1.15**<br>**36.46**<br>**0.915** |

-----
