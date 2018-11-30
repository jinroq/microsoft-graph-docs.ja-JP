---
title: 招待マネージャー
description: '招待マネージャーを使用して、組織に外部ユーザーを追加するための招待状を作成します。 '
ms.openlocfilehash: c8b8bacaf85c36f24ec89b05594ff0880fa8c14e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020474"
---
# <a name="invitation-manager"></a>招待マネージャー

招待マネージャーを使用して、組織に外部ユーザーを追加するための招待状を作成します。 

招待処理では、次のフローが使用されます。

* 招待状が作成されます。
* 招待状が招待ユーザーに送信されます (招待状リンクを含む)。
* 招待ユーザーが招待状リンクをクリックしてサインインし、招待状を引き換え、招待ユーザーを表すユーザー エンティティの作成が完了します。
* 引き換えが完了した後、特定のページにユーザーがリダイレクトされます。

招待状を作成すると、応答で引き換え URL が返されます (*inviteRedeemUrl*)。招待状作成 API では、*sendInvitationMessage* を true に設定することにより、引き換え URL を含むメールが自動的に招待ユーザーに送信されます。招待ユーザーに送信されるメッセージをカスタマイズすることもできます。代わりに、他の手段で引き換え URL を送信したい場合は、*sendInvitationMessage* を false に設定し、応答からの引き換え URL を使用して、独自の通信を作成することもできます。現在、引き換え処理を実行するための API はありません。招待ユーザーは、上記手順の通信で送信された *inviteRedeemUrl* リンクをクリックして、対話型引き換え処理をブラウザーで行う必要があります。完了すると、招待ユーザーは、組織における外部ユーザーになります。


## <a name="methods"></a>メソッド
| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[招待状の作成](../api/invitation-post.md) | invitation | 招待状オブジェクトのプロパティと関係を書き込みます。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|invitedUserDisplayName|String|招待されるユーザーの表示名。|
|invitedUserEmailAddress|String|招待されるユーザーのメール アドレス。必須。|
|invitedUserMessageInfo|[invitedUserMessageInfo](invitedusermessageinfo.md)|メッセージ テキスト、言語、および cc 受信者リストのカスタマイズなど、招待ユーザーに送信されるメッセージの追加構成。|
|sendInvitationMessage|ブール値|招待されるユーザーにメールを送信するかどうかを示します。既定値は false です。|
|inviteRedirectUrl|String|招待状が引き換えられるとにユーザーがリダイレクトされる URL。必須。|
|inviteRedeemUrl|String|ユーザーが招待状の引き換えに使用できる URL。読み取り専用|
|invitedUserType|String|招待されるユーザーの userType。 既定では Guest です。 会社の管理者の場合は、Member として招待できます。 |
|status|String|招待の状態。可能な値:PendingAcceptance、Completed、InProgress、および Error|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|invitedUser|[User](user.md)|招待状作成の一環として作成されたユーザー。読み取り専用|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

<!-- { "blockType": "resource", "baseType": "microsoft.graph.entity", "@odata.type": "microsoft.graph.invitation" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",
  "invitedUser": {"@odata.type": "microsoft.graph.user"},
  "invitedUserType": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
