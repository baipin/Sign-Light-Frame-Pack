# StreetPole 导入修复版

请导入本目录 `StreetPole_Prop`，不要导入旧的 `StreetPole_CS2` 目录。

## 关键修复

- 资产按 **Static Object / Prop** 导入
- 主 FBX：`StreetPole.fbx`
- 主网格对象名：`StreetPole`
- 网格数据名：`StreetPole`
- 原点位于柱体底部，局部 Z 范围为 `0–3 m`
- 尺寸：`0.12 × 0.12 × 3.0 m`
- 目录中没有外部 LOD FBX，LOD 由 `settings.json` 自动生成

## 导入步骤

1. 关闭之前的导入任务，必要时重启资产编辑器。
2. 选择整个 `StreetPole_Prop` 文件夹。
3. 资产类型选择 **Static Object / Prop**，不要选择建筑、道路网络或其他资产类型。
4. 确认主文件是 `StreetPole.fbx`。
5. LOD1 设置为 50%，LOD2 设置为 20%。
6. 只点击一次 Import，等待完成。
7. 导入完成后，在资产浏览器中搜索 `StreetPole`，从道具/静态物体分类中选择它，再点击道路或地面放置。

如果导入后没有放置交互，通常是资产类型没有选为 Prop，或者编辑器仍使用旧的空预制件缓存。重启资产编辑器后只导入本目录，不要同时导入旧版本。
