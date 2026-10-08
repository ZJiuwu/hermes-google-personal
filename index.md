---
layout: default
title: Hermes — Jiuwu 的个人 Google 助手
---

# Hermes — Jiuwu 的个人 Google 助手

Hermes 是由 Jiuwu（GitHub：ZJiuwu）自行部署、仅供个人使用的 AI 助手。本网站说明该个人部署如何连接 Google 服务，不是 Google 或 Nous Research 的官方网站，也不对公众提供注册或授权服务。

## 用途

用户通过聊天向助手下达任务。经用户 OAuth 授权后，助手可查询、总结邮件，管理日历，查找和处理 Drive 文件，读取或编辑 Google 表格和文档，以及查询联系人。

涉及邮件发送、内容修改、删除或文件共享的操作，助手按用户要求先确认再执行。OAuth 权限本身并不会强制这种逐次确认；这是个人部署的操作规则。

## 使用的服务与权限

- Gmail：读取邮件、发送邮件、修改邮件及标签。
- Google Calendar：读取和管理日历、日程。
- Google Drive：读取和管理授权账号可访问的文件，包括内容和共享设置。
- Google Sheets：读取和编辑表格。
- Google Docs：读取和编辑文档。
- Google Contacts（People API）：只读联系人。

完整 Drive、日历及邮件修改权限的能力范围大于单个测试文件。本部署仅按用户指令使用，不将权限描述为只读。

## 数据处理

Google 内容通过个人部署的 Hermes 服务器处理。完成用户请求时，相关内容可能提交给配置的 AI 模型服务，并通过配置的聊天平台返回结果。详细说明见[隐私政策](privacy.html)。

## 撤销访问

用户可在 [Google 账号的第三方连接](https://myaccount.google.com/connections)中撤销 Hermes 的授权。撤销会阻止后续 API 访问，但不会自动清除已经保存在本地、聊天记录或备份中的副本。

## 联系与维护

维护者：[ZJiuwu](https://github.com/ZJiuwu)。可通过本项目的 [GitHub Issues](https://github.com/ZJiuwu/hermes-google-personal/issues)联系。请勿在公开 Issue 中提交邮件内容、授权码、令牌或其他敏感信息。

本应用基于 [Nous Research 的 Hermes Agent](https://github.com/NousResearch/hermes-agent)；本网站仅代表 Jiuwu 的个人部署。
