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

| Method Name       | Original Repository                          | Paper Citation       |
|-------------------|---------------------------------------------|----------------------|
| Method A          | [github.com/original/repoA](url)            | Author et al., 2020  |
| Method B          | [github.com/original/repoB](url)            | Author et al., 2021  |
| Method C          | [github.com/original/repoC](url)            | Author et al., 2022  |
## MIF Method📚 Source Code References

| Method Name       | Original Repository                          | Paper Citation       |
|-------------------|---------------------------------------------|----------------------|
| Method A          | [github.com/original/repoA](url)            | Author et al., 2020  |
| Method B          | [github.com/original/repoB](url)            | Author et al., 2021  |
| Method C          | [github.com/original/repoC](url)            | Author et al., 2022  |
## MFIF Method📚 Source Code References

| Method Name       | Original Repository                          | Paper Citation       |
|-------------------|---------------------------------------------|----------------------|
| Method A          | [github.com/original/repoA](url)            | Author et al., 2020  |
| Method B          | [github.com/original/repoB](url)            | Author et al., 2021  |
| Method C          | [github.com/original/repoC](url)            | Author et al., 2022  |
## UNIVERSAL Method📚 Source Code References

| Method Name       | Original Repository                          | Paper Citation       |
|-------------------|---------------------------------------------|----------------------|
| Method A          | [github.com/original/repoA](url)            | Author et al., 2020  |
| Method B          | [github.com/original/repoB](url)            | Author et al., 2021  |
| Method C          | [github.com/original/repoC](url)            | Author et al., 2022  |






