# Bi-Attention-Net
Improvement of  famous real-time image segmentation paper: BiSeNet.

In recent years, semantic segmentation is a very important issue in image processing. Most of the mobile applications of sematic segmentation require real time.  We call it real-time semantic segmentation. In real-time semantic segmentation, it is always a tough decision between accuracy and inference time. Therefore, there is Bi-Attention Network, utilizing efficient attention modules and truncating branches form former layers. The work achieves 70.6% mean-IoU (mean intersection of union) in Cityscapes dataset with 80.64 FPS (frame per second) which are 1% and 13% improved form BiSeNet. Beside them, we also save 11% of the memory usage.

# Architecture:  
Overall
![overall](https://user-images.githubusercontent.com/28528165/144934831-dea907b3-7151-4c1a-91c5-82fcf46e1102.png)

Spatial attention block and Channel attention block in Overall  
<img src="https://user-images.githubusercontent.com/28528165/144935869-f1277c30-f58f-4767-ae9d-419a16042032.png" width="300" height="300">
<img src="https://user-images.githubusercontent.com/28528165/144935926-6d15a6aa-3cfd-4f80-994d-f411ee8ed924.png" width="300" height="300">


# Experiment and Results:  
Comparison with other works in CityScapes evaluation set (training batch size=4):  
A|Mean-IoU(%)|FPS(frame)
--- | --- | ---
ENet|58.3|76.9
ESPNet|60.36|67.56
BiSeNet|69.26|71.42
Bi-Attention Net|70.61|80.64

![comparison_city](https://user-images.githubusercontent.com/28528165/144938516-fc25c27b-b221-45a2-80b3-189e1b876565.png)

