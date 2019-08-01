---
title: Microsoft Graph API を使用して変更通知を取得する
description: Microsoft Graph の REST API は、webhook メカニズムを使用して、クライアントに変更通知を配信します。 クライアントは、通知を受信するために自身の URL を構成する Web サービスです。 クライアント アプリは通知を使用して、変更時に状態を更新します。 着信通知のサブスクライブ方法や処理方法などの詳細については、「ユーザー データの変更に関する通知の設定」をご覧ください。
localization_priority: Priority
author: piotrci
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 1722f888cc7e29e958a84720f8e714f2379db7da
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033405"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Microsoft Graph API を使用して変更通知を取得する

Microsoft Graph の REST API は、webhook メカニズムを使用して、クライアントに変更通知を配信します。 クライアントは、通知を受信するために自身の URL を構成する Web サービスです。 クライアント アプリは通知を使用して、変更時に状態を更新します。 着信通知のサブスクライブ方法や処理方法などの詳細については、「[ユーザー データの変更に関する通知の設定](/graph/webhooks)」をご覧ください。

Microsoft Graph の API を使用すると、アプリは次のリソースの変更にサブスクライブできます。

- Outlook [メッセージ][]
- Outlook [イベント][]
- Outlook 個人用[連絡先][]
- [ユーザー][]
- [グループ][]
- Office 365 グループ[会話][]
- ユーザーの個人用 OneDrive 上の_任意のフォルダーの_ [driveItem][] 階層内のコンテンツ
- OneDrive for Business 上の_ルート フォルダーの _ [driveItem][] 階層内のコンテンツ
- セキュリティの[警告][]

## <a name="permissions"></a>アクセス許可

一般に、サブスクリプション操作にはリソースへの読み取りアクセス許可が必要です。 たとえば、メッセージの通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。 記事「[サブスクリプションを作成する](../api/subscription-post-subscriptions.md)」では、リソースの種類ごとに必要なアクセス許可がリストされています。 次の一覧表に、アプリが特定のリソースの種類に対して Webhook を使用するために要求できるアクセス許可の種類を示します。

| アクセス許可の種類                        | サポートされているリソースの種類                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| 委任 - 職場または学校アカウント     | [警告][]、[連絡先][]、[会話][]、[driveItem][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]|
| 委任 - 個人用の Microsoft アカウント | [連絡先][]、[driveItem][]、[イベント][]、[メッセージ][]                                        |
| アプリケーション                            | [警告][]、[連絡先][]、[driveItem][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]|


## <a name="see-also"></a>関連項目

- [サブスクリプション リソースの種類](./subscription.md)
- [サブスクリプションのリスト作成](../api/subscription-list.md)
- [サブスクリプションの取得](../api/subscription-get.md)
- [サブスクリプションの作成](../api/subscription-post-subscriptions.md)
- [サブスクリプションの更新](../api/subscription-update.md)
- [サブスクリプションの削除](../api/subscription-delete.md)

[連絡先]: ./contact.md
[会話]: ./conversation.md
[driveItem]: ./driveitem.md
[イベント]: ./event.md
[グループ]: ./group.md
[メッセージ]: ./message.md
[ユーザー]: ./user.md
[警告]: ./alert.md
