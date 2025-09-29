# UniFusion
# Benchmark 评估平台使用说明

## 平台功能

提供两个核心评估界面：

1. **单方法性能测试界面**  
   - 测试指定方法在特定场景下的性能指标
   - 输出结果包括：FLOPS/参数量/平均运行时间
   - 自动保存融合结果到`results/方法名/`

2. **多方法对比界面**  
   - 对同一场景下各方法的融合指标结果进行综合比对
   - 仅通用方法会进行跨场景评估
   - 专用方法只在预设场景下显示


## 平台适配代码
本平台仅提供：
- 📌 二次开发的**指标统计模块**
- 📌 适配本平台的**接口对接代码**

## 完整代码获取
1. 原始方法请访问各项目原仓库
2. 完整适配版本（含依赖调整）请联系本平台作者获取



  
## ⚠️ 性能注意事项

**由于网络通信和硬件性能限制，使用时可能出现：**
- 加载界面显示短暂卡顿
- 指标文件生成延迟（约10-30秒不等）
- 多方法对比时的加载等待

> 演示GIF中已包含这些正常现象的表现，请以实际运行情况为准


# 基准测试方法源码引用说明

## 开源方法引用
所有基准方法的原始代码均来自以下GitHub仓库：

## IVIF Methods📚 Source Code References

| Method Name       | Original Repository                               | Paper Citation                                                                                                                                                                                                                           |
|-------------------|---------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| RFN-Nest          |[https://github.com/hli1221/imagefusion-rfn-nest]  | Li et al., Rfn-nest: An end-to-end residual fusion network for infrared and visible images. Information Fusion,73:72–86, 2021.                                                                                                           |
| UNFusion          | [https://github.com/Zhishe-Wang/UNFusion]         | Wang et al.,Unfusion: A unified multi-scale densely connected network forinfrared and visible image fusion. IEEE Transactions on Circuits and Systems for Video Technology, 32(6):3360–3374, 2021.                                       |
| SuperFusion       | [https://github.com/Linfeng-Tang/SuperFusion]     | Tang et al., Superfusion: A versatile image registration and fusion network with semantic awareness. IEEE/CAA Journal of Automatica Sinica, 9(12):2121–2137, 2022.                                                                       |
| ReCoNet           | [https://github.com/dlut-dimt/ReCoNet]            | Huang et al., Reconet: Recurrent correction network for fast and efficient multi-modality image fusion. In European conference on computer Vision, pages 539–555. Springer, 2022.                                                        |
| SeAFusion         | [https://github.com/Linfeng-Tang/SeAFusion]       | Tang et al., Image fusion in the loop of high-level vision tasks: A semantic-aware real-time infrared and visible image fusion network. Information Fusion, 82:28–42, 2022.                                                              |
| PIAFusion         | [https://github.com/Linfeng-Tang/PIAFusion]       | Tang et al., Piafusion: A progressive infrared and visible image fusion network based on illumination aware. Information Fusion, 83:79–92, 2022.                                                                                         |
| DATFuse           | [https://github.com/tthinking/DATFuse]            | Tang et al., Datfuse: Infrared and visible image fusion via dual attention transformer. IEEE Transactions on Circuits and Systems for Video Technology, 33(7):3159–3172, 2023.                                                           |
| PSFusion          | [https://github.com/Linfeng-Tang/PSFusion]        | Tang et al., Rethinking the necessity of image fusion in high-level vision tasks: A practical infrared and visible image fusion network based on progressive semantic injection and scene fidelity. Information Fusion, 99:101870, 2023. |
| MetaFusion        | [https://github.com/wdzhao123/MetaFusion]         | Zhao et al., Metafusion: Infrared and visible image fusion via meta-feature embedding from object detection. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, pages 13955–13965, 2023.              |
| SDCFusion         | [https://github.com/XiaoW-Liu/SDCFusion]          | Liu et al., A semantic-driven coupled network for infrared and visible image fusion. Information Fusion, 108:102352, 2024                                                                                                                |
| Text-IF           | [https://github.com/XunpengYi/Text-IF]            | Yi et al., Text-if: Leveraging semantic text guidance for degradation-aware and interactive image fusion. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, pages 27026–27035,2024.                  | 
| PromptFusion      | [https://github.com/hey-it-s-me/PromptFusion]     | Liu et al., Promptfusion: Harmonized semantic prompt learning for infrared and visible image fusion. IEEE/CAA Journal of Automatica Sinica, 2024.                                                                                        |
| Conti-Fuse        | [https://github.com/zipper112/Conti-Fuse]         | Li et al., Conti-fuse: A novel continuous decomposition-based fusion framework for infrared and visible images. Information Fusion, 117:102839, 2025.                                                                                    |
| CrossFuse         | [https://github.com/CidanShi/CrossFuse]           | Shi et al., Crossfuse: Learning infrared and visible image fusion by cross-sensor top-k vision alignment and beyond. IEEE Transactions on Circuits and Systems for Video Technology, 2025.                                               |

## MIF Method📚 Source Code References

| Method Name       | Original Repository                                 | Paper Citation       |
|-------------------|-----------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------|
| BSAFusion        | [https://github.com/slrl123/BSAFusion]                   | Li et al., Bsafusion: A bidirectional stepwise feature alignment network for unaligned medical image fusion. In Proceedings of the AAAI Conference on Artificial Intelligence, volume 39, pages 4725–4733, 2025.  |
| GeSeNet       | [https://github.com/lok-18/GeSeNet]                   |Li et al., Gesenet: A general semantic-guided network with couple mask ensemble for medical image fusion. IEEE Transactions on Neural Networks and Learning Systems, 2023.  |
| MACTFusion          | [https://github.com/millieXie/MACTFusion]                   | Xie et al., Mactfusion: Lightweight cross transformer for adaptive multimodal medical image fusion. IEEE Journal of Biomedical and Health Informatics, 2024.  |
| MRSCFusion        | [https://github.com/millieXie/MRSCFusion]                  | Xie et al.,  Mrscfusion: Joint residual swin transformer and multiscale cnn for unsupervised multimodal medical image fusion. IEEE Transactions on Instrumentation and Measurement, 72:1–17, 2023. |
 |MsgFusion         | [https://github.com/22385wjy/MsgFusion]                   | Wen et al., Msgfusion: Medical semantic guided two-branch network for multimodal brain image fusion. IEEE Transactions on Multimedia, 26:944–957, 2023.  |
 |MSRPAN          | [https://github.com/jeffsonfu/MSRPAN]                  | Fu et al.,  A multiscale residual pyramid attention network for medical image fusion. Biomedical Signal Processing and Control, 66:102488, 2021.  |
 |Zero-LMF      | [https://github.com/PanPapag/Zero-Learning-Fast-Medical-Image-Fusion]                   | Fayez Lahoud and Sabine Süsstrunk. Zero-learning fast medical image fusion. In 2019 22th international conference on information fusion (FUSION), pages 1–8. IEEE, 2019. |
 |MATR         | [https://github.com/tthinking/MATR]                   | Tang et al., Matr: Multimodal medical image fusion via multiscale adaptive transformer. IEEE Transactions on Image Processing, 31:5134–5149, 2022.  |
 |FATFusion         | [https://github.com/tthinking/FATFusion]                  | Tang et al., Fatfusion: A functional–anatomical transformer for medical image fusion. Information Processing & Management, 61(4):103687, 2024.  |

## MFIF Method📚 Source Code References

| Method Name       | Original Repository                                  | Paper Citation       |
|-------------------|------------------------------------------------------|----------------------|
| DRPL                | [https://github.com/sasky1/DRPL]                   | Li et al., Drpl: Deep regression pair learning for multifocus image fusion. IEEE Transactions on Image Processing, 29:4816–4831, 2020.  |
| MCCSR-Net         | [https://github.com/yuliu316316/CCSR-Net-Fusion]                    | Zheng et al.,  Unfolding coupled convolutional sparse representation for multi-focus image fusion. Information Fusion, 118:102974, 2025. |
| MFFT          | [https://github.com/zwy0913/MFFT]                    | Zhai et al.,  Multi-focus image fusion via interactive transformer and asymmetric soft sharing. Engineering Applications of Artificial Intelligence, 133:107967, 2024. |
| ZMFF       | [https://github.com/junjun-jiang/ZMFF]                  | Hu et al.,  Zmff: Zero-shot multi-focus image fusion. Information Fusion, 92:127–138, 2023.                                                                                                |
| MFIF-GAN         | [https://github.com/ycwang-libra/MFIF-GAN]                    | Wang et al., Mfif-gan: A new generative adversarial network for multi-focus image fusion. Signal Processing: Image Communication, 96:116295, 2021.               |
| SESF-Fuse         | [https://github.com/Keep-Passion/SESF-Fuse]                    | Ma et al., Sesf-fuse: An unsupervised deep model for multi-focus image fusion. Neural Computing and Applications, 33(11):5793–5804, 2021. |
## UNIVERSAL Method📚 Source Code References

| Method Name       | Original Repository                                  | Paper Citation       |
|-------------------|------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| SwinFusion          | [https://github.com/Linfeng-Tang/SwinFusion]                    |Ma et al.,  Swinfusion: Cross-domain long-range learning for general image fusion via swin transformer. IEEE/CAA Journal of Automatica Sinica, 9(7):1200–1217, 2022.                                                                                          |
| DDFM          | [https://github.com/Zhaozixiang1228/MMIF-DDFM]                    | Zhao et al., Ddfm: denoising diffusion model for multi-modality image fusion. In Proceedings of the IEEE/CVF international conference on computer vision, pages 8082–8093, 2023                                                                       |
| CDDFuse         | [https://github.com/Zhaozixiang1228/MMIF-CDDFuse]                    | Zhao et al., Cddfuse: Correlation-driven dual-branch feature decomposition for multi-modality image fusion. In Proceedings of the IEEE/CVF conference on computer vision and pattern recognition, pages 5906–5916, 2023.  |
| EMMA          | [https://github.com/Zhaozixiang1228/MMIF-EMMA]                    | Zhao et al., Equivariant multi-modality image fusion. In Proceedings of the IEEE/CVF conference on computer vision and pattern recognition, pages 25912–25921, 2024.                                                                                       |
| TIM          | [https://github.com/LiuZhu-CV/TIMFusion]                    | Liu et al.,  A task-guided, implicitly-searched and meta-initialized deep model for image fusion. IEEE Transactions on Pattern Analysis and Machine Intelligence, 46(10):6594–6609, 2024.                                                           |
| MMAE        | [https://github.com/xiangxiang-wang/MMAE]                   | Wang et al.,  Mmae: A universal image fusion method via mask attention mechanism. Pattern Recognition, 158:111041, 2025.                                                                                                                                                          |
|LFDT-Fusion           | [https://github.com/BOYang-pro/LFDT-Fusion]                     | Yang et al.,  Lfdt-fusion: A latent feature-guided diffusion transformer model for general image fusion. Information Fusion, 113:102639, 2025.                                                                                                                                   |
| MMIF-INet          | [https://github.com/HeDan-11/MMIF-INet]               | He et al.,  Mmif-inet: Multimodal medical image fusion by invertible network. Information Fusion, 114:102666, 2025.  |






