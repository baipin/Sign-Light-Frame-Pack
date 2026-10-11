# Pole_As_SignLight_Structure

这是用于验证 CS2 资产解析的诊断包。它使用已经确认可正常导入的 SignLight FBX 结构，只把几何替换为 3 m 路牌柱。

## 导入

1. 重启资产编辑器。
2. 导入整个本目录。
3. 选择 **Static Object / Prop**。
4. 主文件必须是 `SignLight.fbx`。
5. 只点击一次 Import。

如果这个版本可以放置，说明问题来自 `StreetPole` 资产名的解析或旧目录缓存；可以在资产编辑器中将导入后的资产改名为 StreetPole。若仍然没有放置交互，则问题在资产编辑器的资产类型/导入缓存，而不是柱体几何或纹理。

模型实际尺寸为 `0.12 × 0.12 × 3.0 m`，原点位于底部，淡蓝灰色材质沿用可用 SignLight 结构。
