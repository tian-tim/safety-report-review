<!-- SPDX-License-Identifier: Apache-2.0 -->
<!-- SPDX-FileCopyrightText: 2026 tianhuan <tianhuan@gumingnc.com> -->

# 规约检查记录

日期：2026-11-04。
范围：只生成规约与提示词，不生成业务代码。

## 格式检查

使用本机Node.js 24.18.0执行已安装的Spex 6.0.0 CLI，工作目录为 D:\AI培训。
实际命令：`D:\develop\nvm\v24.18.0\node.exe D:\develop\nvm\v16.20.0\node_modules\@sublang\spex\dist\cli.js lint`。
结果：退出码0，`spex lint: no problems found`，无错误或警告。

## 内容审阅

- 已覆盖上传、三位专家独立邀请、意见与确认签署、个人及整体状态。
- EER-001～003已映射至三个正式行为条目。
- 已编写V01～V16系统验收场景，业务系统未实现，尚未执行这些场景。
- 已保留用户要求的三文件交付目录，规范性内容采用Spex 6单文件包。
- 未修改受保护的meta.md，未变更全局Node.js版本。
- 人工需审阅姓名签署假设，以及邀请通道、文件限制、邀请有效期和身份验证方式。

## 飞书提示词

本地提示词：`docs/expert-review-prompt.md`。
飞书用户授权已完成，提示词已创建并回读核验，标题及六个章节完整。
飞书文档：[https://rcnbdd2w7hg8.feishu.cn/docx/OqtGd1aIioDvsexFxcKcUoMMnce](https://rcnbdd2w7hg8.feishu.cn/docx/OqtGd1aIioDvsexFxcKcUoMMnce)。