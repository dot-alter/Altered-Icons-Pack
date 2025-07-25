# 构建度量标准  
<small>阅读时间：3 分钟</small>

**本节内容**
+ [尺寸 ↴](#-尺寸)
+ [描边 ↴](#-描边)
+ [圆角 ↴](#-圆角)

---

## 〰️ 描边

描边厚度是保持视觉一致性和在不同尺寸下易读性的关键。我们使用 `1.5dp` 的描边宽度，应用于曲线与端点，描边**向图形内部对齐**。

Altered Icons 的一大特色是 **独立描边模拟**。即，不直接使用标准的 `1.5dp` 线条，而是构建一个完整的图形轮廓，模拟线条路径并增加视觉厚度和体积。

![Al-plus-icon comparison](../../.github/assets/Al-plus-icon-comparison.webp)

仅当常规描边不符合图标风格或破坏整体视觉协调时，才会采用此方法。

---

## ↪️ 圆角

图标的圆角基于 `24×24dp` 的网格系统。对于方形、矩形或三角形图形，其角部半径为 `2dp`。

![corner-shape-grid](../../.github/assets/corner-rectangle-grid.jpg)

而对于近似圆形的图形（不一定为完美圆形），角部半径设置为 `4dp`，并根据网格中的基础圆形调整曲线，以生成目标形状。

![circle-corner-grid](../../.github/assets/circle-corner-grid.jpg)

在描边的体积处理中，边缘厚度可延展至 `1dp`。

![shape-volume-grid](../../.github/assets/shape-volume-grid.jpg)

---

## 📍 相关链接

**前一节**
+ [图标设计 →](./02_design.md)
+ [集合原则 →](./01_principles.md)

**其他**
+ [如何贡献 →](./CONTRIBUTING.md)