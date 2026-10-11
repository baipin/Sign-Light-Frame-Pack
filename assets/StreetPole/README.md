# StreetPole_Prop_Clean

这是用于排查 CS2 资产编辑器放置问题的最小 Prop 版本。

## 内容

- `StreetPole.fbx`：唯一主模型，直接包含淡蓝灰色哑光材质
- `settings.json`：LOD1=50%，LOD2=20%
- `IMPORT_THIS.txt`：导入提示

本版本故意不包含外部 PNG、外部 LOD FBX 或其他材质文件，避免纹理解析失败导致资产预制件没有创建。

## FBX 结构

- 文件名：`StreetPole.fbx`
- 对象名：`StreetPole`
- 网格数据名：`StreetPole_LOD0_Mesh`
- 材质名：`StreetPole_Painted`
- 尺寸：`0.12 × 0.12 × 3.0 m`
- 原点：柱体底部，局部 Z 范围 `0–3 m`
- 坐标：Forward `-Y`，Up `Z`
- 材质：淡蓝灰色、Metallic=0、Roughness=0.82

## 导入

1. 重启资产编辑器，避免旧的空预制件缓存。
2. 选择整个 `StreetPole_Prop_Clean` 文件夹。
3. 资产类型必须选择 **Prop** 或 **Static Object**。
4. 不要选择建筑、道路或网络资产类型。
5. 只导入 `StreetPole.fbx`，不要添加其他 FBX。
6. 导入完成后保存资产，再从 Props / 道具分类中选择 `StreetPole` 放置。

如果这个最小版本能够放置，说明之前的问题来自外部纹理或纹理组解析；之后再把 `StreetPole_BaseColor.png` 作为可选纹理逐步加入。
