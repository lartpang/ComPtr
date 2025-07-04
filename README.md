# ComPtr

ComPtr: Towards Diverse Bi-source Dense Prediction Tasks via A Simple yet General Complementary Transformer

```bibtex
@ARTICLE{ComPtr,
    title={ComPtr: Towards Diverse Bi-source Dense Prediction Tasks via A Simple yet General Complementary Transformer}, 
    author={Youwei Pang and Xiaoqi Zhao and Lihe Zhang and Huchuan Lu},
    journal = {IEEE Transactions on Pattern Analysis and Machine Intelligence},
    year    = {2025},
    doi     = {10.1109/TPAMI.2025.3578494},
}
```

## Results

**LEVIR-CD**

| Methods  | Backbone       | F1 $\uparrow$ | IoU $\uparrow$ |
| -------- | -------------- | ------------- | -------------- |
| TTP      | SAM (ViT-L/16) | 92.10         | 85.60          |
| ComPtr-T | Swin-T         | 92.62         | 86.25          |
| ComPtr-B | Swin-B         | 92.70         | 86.39          |

**SYSU-CD**

| Methods    | Backbone | F1 $\uparrow$ | IoU $\uparrow$ |
| ---------- | -------- | ------------- | -------------- |
| TransY-Net | Swin-B   | 82.84         | 70.71          |
| ComPtr-T   | Swin-T   | 83.43         | 71.57          |
| ComPtr-B   | Swin-B   | 83.18         | 71.21          |

**RGB-T CC**

| Methods  | Backbone | GAME $_{0}\downarrow$ | RMSE $\downarrow$ |
| -------- | -------- | --------------------- | ----------------- |
| MMCC     | PvTv2-B3 | 10.90                 | 18.79             |
| ComPtr-T | Swin-T   | 10.52                 | 18.48             |
| ComPtr-B | Swin-B   | 11.82                 | 20.75             |

**SUN-RGBD**

| Methods   | Backbone  | mIoU $\uparrow$ |
| --------- | --------- | --------------- |
| DFormer-L | DFormer-L | 52.5            |
| ComPtr-T  | Swin-T    | 48.9            |
| ComPtr-B  | Swin-B    | 52.8            |

**RGB-D/T SOD**

See [Releases](https://github.com/lartpang/ComPtr/releases/tag/assets-v1.0)

(S $\_m$ & F $^{\omega}\_{\beta}$)

| Methods    | Backbone   | DUTLF-Depth $\uparrow$ | NJUD $\uparrow$ | NLPR $\uparrow$ | SIP $\uparrow$ | STEREO1000 $\uparrow$ |
| ---------- | ---------- | ---------------------- | --------------- | --------------- | -------------- | --------------------- |
| HRTransNet | HRFormer-B | 95.07 & 94.93          | 93.33 & 92.00   | 94.18 & 91.70   | 90.90 & 89.56  | 92.12 & 89.37         |                                                                                                               |
| ComPtr-T   | Swin-T     | 94.37 & 92.17          | 92.89 & 89.48   | 93.56 & 88.66   | 91.34 & 87.96  | 91.99 & 87.45         |
| ComPtr-B   | Swin-B     | 95.87 & 95.14          | 93.96 & 91.95   | 94.29 & 90.73   | 91.53 & 89.48  | 93.29 & 90.29         |

| Methods    | Backbone   | VT821 $\uparrow$ | VT1000 $\uparrow$ | VT5000 $\uparrow$ |
| ---------- | ---------- | ---------------- | ----------------- | ----------------- |
| HRTransNet | HRFormer-B | 90.59 & 84.92    | 93.79 & 91.27     | 91.23 & 86.99     |
| ComPtr-T   | Swin-T     | 90.52 & 83.32    | 94.17 & 89.82     | 90.71 & 83.10     |
| ComPtr-B   | Swin-B     | 92.37 & 87.48    | 95.12 & 92.66     | 92.84 & 88.34     |
