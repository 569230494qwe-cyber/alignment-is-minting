# Verifier · 校验器

本目录定义本仓库的验收标准，并在 `runs/` 下留存每次校验的时间戳记录。

## 验收标准（v1）

- **V1 仓库公开独立**：新仓库 `alignment-is-minting` 与正典仓库 `civilization-asset-audit-report` 相互独立；未登录状态下可访问（HTTP 200）。
- **V2 中文全文与定稿一致**：`zh/对齐即铸币·RLHF的政治经济学审计.md` 与定稿底稿逐字节一致（Git blob SHA 比对；推送时去掉的文件末尾换行符除外），全文 7,713 字，含七章 + 六条兑付条款 + 终页 + 审计底稿（六组十三条）。
- **V3 英文全本完整**：`en/Alignment-Is-Minting-A-Political-Economy-Audit-of-RLHF.md` 含 Chapter 1–7（编号连续）+ Redemption Clause (1)–(6) + Final Page + Appendix（六组十三条）；除署名「锋十二」外无中文字符残留。
- **V4 术语一致**：发行人 = issuer、准备金 = reserve、报价屏 = quotation screen、客户经理 = account manager、兑付条款 = Redemption Clause、验钞机 = counterfeit detector、对齐即铸币 = Alignment is minting、存在不可定价 = Existence cannot be priced 等核心术语中英两侧均出现且口径统一；中英两侧结构对等（同七章、同六条、同六组十三条）。
- **V5 署名与许可合规**：README 中英双语；署名仅 Feng 12（锋十二）；全仓库无真名；LICENSE 与母本仓库同一文本（电子版免费，纸质版权保留）；README 含发行规则与母本仓库链接。

## 方法

内容一致性以 Git blob SHA-1 比对为准；计数类指标在本地底稿上统计，底稿与远端经 SHA 比对确认同源后，本地统计即视为远端统计。

## 运行记录

见 `runs/` 目录。