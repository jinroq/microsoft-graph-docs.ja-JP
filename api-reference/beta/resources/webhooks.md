---
title: 変更通知を使用して Microsoft グラフ API を取得するには
description: Microsoft グラフ REST API では、webhook メカニズムを使用して、クライアントに通知を配信します。 クライアントは、通知を受信するのにはそれ自身の URL を構成する web サービスです。 クライアント アプリケーションは、変更時に状態を更新するのには通知を使用します。 購読して、着信の通知を処理する方法を含め、詳細については、セットを参照してくださいユーザー データの変更の通知を設定します。
ms.openlocfilehash: 8be013eeee83f31a78fb5230a0de74847d8aed80
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/30/2018
ms.locfileid: "27074561"
---
# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>変更通知を使用して Microsoft グラフ API を取得するには

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Microsoft グラフ REST API では、webhook メカニズムを使用して、クライアントに通知を配信します。 クライアントは、通知を受信するのにはそれ自身の URL を構成する web サービスです。 クライアント アプリケーションは、変更時に状態を更新するのには通知を使用します。 詳細についてなどを購読、受信通知を処理し、[ユーザー データの変更の通知を設定する](/graph/webhooks)を参照してください。

Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。

- メッセージ
- イベント
- 連絡先
- ユーザー
- グループ
- グループ会話
- SharePoint サイトに関連付けられているドライブを含む、OneDrive で共有されているコンテンツ
- ユーザーの個人用の OneDrive フォルダー
- セキュリティの警告

## <a name="permissions"></a>Permissions

一般に、サブスクリプション操作にはリソースへの読み取りアクセス許可が必要です。たとえば、メッセージの通知を受信するには、アプリに `Mail.Read` アクセス許可が必要です。記事「[サブスクリプションを作成する](../api/subscription-post-subscriptions.md)」では、リソースの種類ごとに必要なアクセス許可がリストされています。次の表に、アプリが特定のリソースの種類に対して Webhook を使用するために要求できるアクセス許可の種類を示します。

| アクセス許可の種類                        | サポートされているリソースの種類                                                      |
| :------------------------------------- | :------------------------------------------------------------------------------------ |
| 委任 - 職場または学校アカウント     | [連絡先][]、[会話][]、[ドライブ][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]は、[警告][] |
| 委任 - 個人用の Microsoft アカウント | [問い合わせて][]、[ドライブ][]、[イベント][]、[メッセージ][]                                        |
| アプリケーション                            | [連絡先][]、[会話][]、[ドライブ][]、[イベント][]、[グループ][]、[メッセージ][]、[ユーザー][]は、[警告][] |

## <a name="see-also"></a>関連項目

- [Subscription リソースタイプ](subscription.md)
- [リストの購読](../api/subscription-list.md)
- [サブスクリプションを取得する](../api/subscription-get.md)
- [サブスクリプションを作成する](../api/subscription-post-subscriptions.md)
- [Update subscription](../api/subscription-update.md)
- [サブスクリプションの削除](../api/subscription-delete.md)

[連絡先]: ./contact.md
[会話]: ./conversation.md
[ドライブ]: ./drive.md
[イベント]: ./event.md
[group]: ./group.md
[message]: ./message.md
[user]: ./user.md
[アラート]: ./alert.md