# 第5章：KDRoi 公式——选词的终极标准

## 为什么需要公式？

选出候选词之后，如何最终决定做哪个？

Semrush 导出的关键词表格可能有几百上千个词，人工一个个判断不现实。

**KDRoi 公式，就是用数据说话。**

## KDRoi 公式

```
KDRoi = (搜索量 × CPC) / 优化难度 KD
```

- **搜索量（Volume）**：代表需求大小
- **CPC（Cost Per Click）**：代表商业价值（广告主愿意付的钱）
- **优化难度（KD）**：代表竞争程度

**KDRoi 越高，这个词越值得做。**

## 实操方法

1. 在 Semrush 搜索主关键词，导出所有相关关键词表格
2. 下载到本地，保留 **Keyword、Volume、KD、CPC** 四列
3. 在 Excel 中新增一列，输入公式：`=B2*D2/C2`
4. 按 KDRoi 从高到低排序
5. 取排名前列的词，再用搜索意图分析

## 实际案例：Calculator

Semrush 搜索 "Calculator"，筛选：
- 搜索量：600+/月
- KD：0-29
- CPC：> $0.1
- 排除 "near me" 关键词

得到 357 个关键词，按 KDRoi 排序后，排名前 10：

| 关键词 | 搜索量 | KD | CPC | KDRoi |
|--------|--------|-----|-----|--------|
| katy hearn macro calculator | 1900 | 0 | 0.98 | ∞ |
| audiobook speed calculator | 1600 | 7 | 13.9 | 3177 |
| audiobook calculator | 1600 | 8 | 12.34 | 2468 |
| neb tm calculator | 5400 | 19 | 5.79 | 1645 |
| shsat score calculator | 1300 | 16 | 12.63 | 1026 |
| construction loan calculator | 6600 | 14 | 1.71 | 806 |
| paycheckcity calculator | 5400 | 18 | 2.64 | 792 |
| sailrite fabric calculator | 720 | 17 | 17.7 | 749 |
| virginia paycheck calculator | 5400 | 29 | 3.95 | 735 |
| oregon paycheck calculator | 5400 | 29 | 3.92 | 729 |

## 什么是好词？

**KDRoi 高的词 = 搜索量不小 + 商业价值高 + 竞争不激烈**

"audiobook speed calculator" 是典型的好词：
- 月搜索量 1600，不算大
- 但 CPC 高达 $13.9，说明广告主愿意为每个点击付 13.9 美元
- KD 只有 7，竞争很小
- KDRoi = 3177，远超其他词

## 注意事项

1. **KDRoi 只是参考**，不是绝对标准。还要结合搜索意图分析。
2. **新词机会**：有些词 KDRoi 不高，但有新词机会，提前占位价值更大。
3. **品牌词**：不要做带品牌名的词，竞争大且法律风险。
4. **不同国家**：同一个词在不同国家的 KDRoi 差异很大，优先做发达国家。

## 自动计算工具

不想手动算？用这个工具自动计算：
https://roi-calculator-flame.vercel.app/

上传 Semrush 导出的 CSV 文件，自动完成计算和排序。
