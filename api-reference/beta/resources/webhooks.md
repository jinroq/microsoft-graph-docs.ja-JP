---
title: Microsoft Graph API を使用して変更通知を取得する
description: Microsoft Graph REST API は、webhook メカニズムを使用して、クライアントに変更通知を配信します。 クライアントは、通知を受信するために自身の URL を構成する Web サービスです。 クライアント アプリは通知を使用して、変更時に状態を更新します。 受信通知をサブスクライブおよび処理する方法などの詳細については、「ユーザーデータの変更の通知を設定する」を参照してください。
localization_priority: Normal
author: piotrci
doc_type: conceptualPageType
ms.prod: ''
ms.openlocfilehash: 8f37e7cfbfe206cfb932661335c78dc370180bac
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964142"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>Microsoft Graph API を使用して変更通知を取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph REST API は、webhook メカニズムを使用して、クライアントに変更通知を配信します。 クライアントは、通知を受信するために自身の URL を構成する Web サービスです。 クライアント アプリは通知を使用して、変更時に状態を更新します。 受信通知をサブスクライブおよび処理する方法などの詳細については、「[ユーザーデータの変更の通知を設定](/graph/webhooks)する」を参照してください。

Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。

- Outlook [メッセージ][]
- Outlook [イベント][]
- Outlook 個人用[連絡先][]
- [user][]
- [group][]
- Office 365 グループ[会話][]
- ユーザーの個人用 OneDrive 上の_任意のフォルダーの_ [driveItem][] 階層内のコンテンツ
- OneDrive for Business 上の_ルート フォルダーの _ [driveItem][] 階層内のコンテンツ
- セキュリティの[警告][]

## <a name="permissions"></a>アクセス許可

一般に、サブスクリプション操作には、リソースに対する読み取りアクセス許可が必要です。 たとえば、メッセージの通知を取得するには、アプリに`Mail.Read`アクセス許可が必要です。 [サブスクリプションの作成](../api/subscription-post-subscriptions.md)の記事には、リソースの種類ごとに必要なアクセス許可が一覧表示されます。 次の表に、特定のリソースの種類に対して webhook を使用するためにアプリが要求できるアクセス許可の種類を示します。

| アクセス許可の種類                        | サポートされるリソースの種類                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| 委任された職場または学校のアカウント     | [通知][]、[連絡先][]、[会話][]、[ドライブアイテム][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]|
| 委任-個人用の Microsoft アカウント | [contact][]、 [drive item][]、 [event][]、 [message][]                                        |
| アプリケーション                            | [alert][]、 [contact][]、 [drive item][]、 [event][]、 [group][]、 [message][]、 [user][]|

## <a name="see-also"></a>関連項目

- [Subscription リソースタイプ](subscription.md)
- [サブスクリプションのリスト作成](../api/subscription-list.md)
- [サブスクリプションを取得する](../api/subscription-get.md)
- [サブスクリプションを作成する](../api/subscription-post-subscriptions.md)
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
