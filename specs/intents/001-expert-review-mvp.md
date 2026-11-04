<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- SPDX-FileCopyrightText: 2026 tianhuan <tianhuan@gumingnc.com> -->

# IR-001：实现三位专家评审签署核心流程

## 状态

规约已编写，待人工审阅；业务实现与系统验收尚未开始。

## 意图

依据 [DR-001](../decisions/001-independent-expert-review.md)，交付管理员上传报告、邀请三位专家、独立评审签署及完成状态汇总的最小流程。

## 交付项

- [x] 一份决策记录与本意图记录。
- [x] 一个正式规约包及三条GEARS行为规约。
- [x] 一套系统验证场景与一条业务流程。
- [x] README.md、rules.md、validation.md 交付目录与可复用提示词。
- [ ] 管理员成功上传报告并可供受邀专家读取。
- [ ] 向三位不同专家分别发送有效邀请。
- [ ] 三位专家独立提交意见、确认并签署。
- [ ] 个人状态与整体状态正确更新。

## 任务

1. 编写并审阅DR、IR、规约、验证场景及索引，运行lint，形成一次文档提交（本次任务，不生成代码）。
2. 人工批准规约后，实现上传及邀请流程，形成一次实现提交（后续）。
3. 实现独立评审、确认签署与状态汇总，形成一次实现提交（后续）。
4. 执行真实系统验收并记录证据，形成一次验收提交（后续）。

## 验证

- 格式：使用Node.js 24执行 `spex lint`，保存实际结果。
- 业务：执行 [[external-expert-review-4](../packages/external-expert-review.md#external-expert-review-4)]、[[external-expert-review-5](../packages/external-expert-review.md#external-expert-review-5)] 和 [[external-expert-review-6](../packages/external-expert-review.md#external-expert-review-6)]。
- 本次仅完成规约设计，不能将格式通过视为系统验收通过。
