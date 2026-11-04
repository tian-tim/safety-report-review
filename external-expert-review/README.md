<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- SPDX-FileCopyrightText: 2026 tianhuan <tianhuan@gumingnc.com> -->

# 外部专家安全报告评审系统——30分钟MVP版

## 项目目标与范围

管理员上传已完成的安全报告，邀请三位外部专家独立评审，各自提交意见、确认并签署，系统汇总完成状态。
本次只交付规约设计，不生成业务代码，不实际发送专家邀请。

## 交付物

| 成果 | 入口 | 数量 |
| --- | --- | --- |
| DR | [决策记录](../specs/decisions/001-independent-expert-review.md) | 1份 |
| IR | [意图记录](../specs/intents/001-expert-review-mvp.md) | 1份 |
| Spec Package | [正式规约包](../specs/packages/external-expert-review.md) | 1个 |
| GEARS行为规约 | [规则索引](rules.md) | 3条 |
| 验证标准 | [验收清单](validation.md) | 1套 |
| 业务流程 | 本文流程 | 1条 |
| 多模型提示词 | [提示词](../docs/expert-review-prompt.md) | 1份 |

## 业务流程

管理员上传报告 → 校验三位专家信息 → 分别发送独立邀请 → 三位专家并行读取报告、提交意见 → 各自确认意见并姓名签署 → 更新个人状态 → 汇总完成数 → 3/3时整体完成。
上传或邀请失败时显示真实失败结果；未完成签署的个人任务不计入完成数。

## 目录约定

本目录保留用户指定的 README.md、rules.md、validation.md 三文件形式。
依据现有 Spex 6 的单文件格式，规范性正文集中于 `specs/packages/external-expert-review.md`，本目录提供阅读入口，避免重复维护。

## 审阅事项

- 已确认：三人独立评审、分别签署、全部完成后整体完成。
- 待审阅假设：MVP签署为姓名加明确确认，不接入证书签章。
- 待实现选型：邀请发送通道、文件类型与大小上限、邀请有效期和身份验证方式。
- 本轮不选定上述技术参数，不宣称系统业务验收已通过。

## 飞书提示词

[打开可复用提示词](https://rcnbdd2w7hg8.feishu.cn/docx/OqtGd1aIioDvsexFxcKcUoMMnce)
