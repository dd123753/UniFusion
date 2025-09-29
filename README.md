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
|-------------------|-----------------------------------------------------|----------------------|
| Method A          | [github.com/original/repoA](url)                    | Author et al., 2020  |
| Method B          | [github.com/original/repoB](url)                    | Author et al., 2021  |
| Method C          | [github.com/original/repoC](url)                    | Author et al., 2022  |
## MFIF Method📚 Source Code References

| Method Name       | Original Repository                                  | Paper Citation       |
|-------------------|------------------------------------------------------|----------------------|
| Method A          | [github.com/original/repoA](url)                     | Author et al., 2020  |
| Method B          | [github.com/original/repoB](url)                     | Author et al., 2021  |
| Method C          | [github.com/original/repoC](url)                     | Author et al., 2022  |
## UNIVERSAL Method📚 Source Code References

| Method Name       | Original Repository                                  | Paper Citation       |
|-------------------|------------------------------------------------------|----------------------|
| Method A          | [github.com/original/repoA](url)                     | Author et al., 2020  |
| Method B          | [github.com/original/repoB](url)                     | Author et al., 2021  |
| Method C          | [github.com/original/repoC](url)                     | Author et al., 2022  |





