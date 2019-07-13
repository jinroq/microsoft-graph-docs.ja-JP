---
title: Microsoft Graph の以前のリリースでの主な変更点
description: Microsoft Graph の以前の新機能
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: e15e68556df2a727e9d40201f892736be066359b
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35420438"
---
# <a name="highlights-of-earlier-releases"></a>以前のリリースでの主な変更点

## <a name="generally-available-released-january---april-2019"></a>一般公開 (2019 年 1 月から 4 月にリリース済み)

[Microsoft Graph データ接続](data-connect-concept-overview.md)

### <a name="calendar"></a>カレンダー
[空き時間のスケジュールを取得する](outlook-get-free-busy-schedule.md)

### <a name="identity-and-access"></a>ID とアクセス
[ID プロバイダー](/graph/api/resources/identityprovider?view=graph-rest-1.0)
[改善された認証ガイド](/graph/auth)
[Azure AD Graph から Microsoft Graph へのアプリの移行](migrate-azure-ad-graph-overview.md)

### <a name="sdks"></a>SDK
[SDK ガイド](/sdks/sdks-overview.md) API スニペット ([例](/graph/api/user-get?view=graph-rest-1.0&tabs=cs#sdk-sample-code))

### <a name="security"></a>セキュリティ
[テナントのセキュア スコア](/graph/api/resources/securescore?view=graph-rest-1.0)

## <a name="preview-released-january---april-2019"></a>プレビュー (2019 年 1 月から 4 月にリリース済み)

### <a name="calendar-group-mail-to-do-tasks"></a>カレンダー、グループ、メール、To Do タスク
イベント、メッセージ、Outlook タスク、グループ投稿での、[添付アイテムまたは添付ファイルの raw/MIME コンテンツの取得](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment)

### <a name="change-notifications"></a>変更通知
[Outlook リソースの変更通知の見逃しを減らす](webhooks-outlook-authz.md)

### <a name="devices-and-apps"></a>デバイスとアプリ
- Intune [1 月](changelog.md#january-2019)の更新プログラム 
- Intune [2 月](changelog.md#february-2019)の更新プログラム
- Intune [3 月](changelog.md#march-2019)の更新プログラム
- Intune [4 月](changelog.md#april-2019)の更新プログラム

### <a name="files"></a>ファイル
有効期限とパスワードを含めることができるようになった[共有の招待](/graph/api/driveitem-invite?view=graph-rest-beta)

### <a name="financials"></a>財務報告
[Dynamics 365 Business Central](dynamics-business-central-concept-overview.md)

### <a name="identity-and-access"></a>ID とアクセス
[アクセス レビュー](/graph/api/resources/accessreviews-root?view=graph-rest-beta) アプリケーション アクセス許可のサポート [監査とサインイン ログ](/graph/api/resources/azure-ad-auditlog-overview?view=graph-rest-beta)
[Azure AD B2C でのカスタム サインインとサインアップ](/graph/api/resources/trustframeworkpolicy?view=graph-rest-beta)
[リスクの高いユーザー](/graph/api/resources/riskyuser?view=graph-rest-beta) および [履歴](/graph/api/resources/riskyuserhistoryitem?view=graph-rest-beta)

### <a name="mail"></a>メール
[メッセージの MIME コンテンツを取得する](outlook-get-mime-message.md)

### <a name="reports"></a>レポート
[アプリケーションのサインイン レポート](/graph/api/resources/applicationsigninsummary?view=graph-rest-beta)

### <a name="security"></a>セキュリティ
[セキュリティ アクション](/graph/api/resources/securityaction?view=graph-rest-beta)
[脅威インジケーター](/graph/api/resources/tiindicator?view=graph-rest-beta)

### <a name="teamwork"></a>チームワーク
[1:1 のチャット](/graph/api/resources/chat?view=graph-rest-beta)
[シフト管理](/graph/api/resources/shift?view=graph-rest-beta)

## <a name="see-also"></a>関連項目
- Microsoft Graph の[最新機能](whats-new-overview.md)を参照してください。
- リリース告知と役に立つリソースについては、「[Microsoft Graph 開発者ブログ](https://developer.microsoft.com/en-us/graph/blogs/)」を定期的に確認してください。
- Microsoft Graph API の追加機能、[更新ログ](changelog.md)の API 動作の更新内容の詳細を参照してください。