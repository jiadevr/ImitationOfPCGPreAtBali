# BaliPCGPre
Imitation Of [Chris Murphy's Pre At Bali Unreal Fest](https://youtu.be/XcL03VkgBH8)
复刻Chris Murphy在UnrealFest2025主旨演讲的道路和城市纯PCG生成项目
[技术分享博客](https://www.bilibili.com/read/cv43780186)
# 结构引导
- PCG为本项目中使用的PCG相关内容
  - SpatialNodeExample:对于CollapsePoints、Attract、Cluster三个关键节点的使用展示
  - PCG_SimpleRoad:道路生成PCG图表
    - PCG_FixConnectTangent:修复道路连接交汇路口部件时的缝隙
  - PCG_SimpleBuilding:建筑生成PCG图表
    - PCG_FloodFill:PCG实现的FloodFill算，用于划分建筑边界，需要注意孤立偏远点可能会无限递归
    - PCG_CreateBuildingFromSpline:对PCG插件中Grammar生成图表的封装，用于根据轮廓生成建筑
  - PCGDataAsset:道路部件LevelInstance和对应的PCGDataAsset资产
- Roads文件下为项目使用的模块化道路免费资产[Modular Roads (Low Poly Style) | Fab-道路资产](https://www.fab.com/zh-cn/listings/8ce6fac4-bb4b-4623-8567-4aee09a80b8d)，该资产模型法线方向是反的，建议直接用本项目中的修复版或者使用UE内建模工具手动修复。 
