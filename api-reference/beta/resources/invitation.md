---
title: 招待リソースの種類
description: 組織に外部ユーザーを追加するために使用される招待を表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a6a009640b47ce02b1719d6e5535813d365dc9e6
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450642"
---
# <a name="invitation-resource-type"></a>招待リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

組織に外部ユーザーを追加するために使用される招待を表します。 

招待処理では、次のフローが使用されます。

* 招待状が作成されます。
* 招待状が招待ユーザーに送信されます (招待状リンクを含む)。
* 招待ユーザーが招待状リンクをクリックしてサインインし、招待状を引き換え、招待ユーザーを表すユーザー エンティティの作成が完了します。
* 引き換えが完了した後、特定のページにユーザーがリダイレクトされます。

招待状を作成すると、応答で引き換え URL が返されます (*inviteRedeemUrl*)。招待状作成 API では、*sendInvitationMessage* を true に設定することにより、引き換え URL を含むメールが自動的に招待ユーザーに送信されます。招待ユーザーに送信されるメッセージをカスタマイズすることもできます。代わりに、他の手段で引き換え URL を送信したい場合は、*sendInvitationMessage* を false に設定し、応答からの引き換え URL を使用して、独自の通信を作成することもできます。現在、引き換え処理を実行するための API はありません。招待ユーザーは、上記手順の通信で送信された *inviteRedeemUrl* リンクをクリックして、対話型引き換え処理をブラウザーで行う必要があります。完了すると、招待ユーザーは、組織における外部ユーザーになります。

>[!NOTE]
>招待の状態は、 **Externaluserstate**と、招待要求の一部として作成された外部[ユーザー](user.md)リソースの**externalUserStateChangeDateTime**プロパティを使用して追跡されます。

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
|sendInvitationMessage|Boolean|招待されるユーザーにメールを送信するかどうかを示します。既定値は false です。|
|inviteRedirectUrl|String|招待状が引き換えられるとにユーザーがリダイレクトされる URL。必須。|
|inviteRedeemUrl|String|ユーザーが招待状の引き換えに使用できる URL。読み取り専用|
|invitedUserType|String|招待されるユーザーの userType。既定では Guest です。会社の管理者は、Member として招待できます。 |
|status|String|招待の状態。可能な値:PendingAcceptance、Completed、InProgress、および Error|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|invitedUser|[ユーザー](user.md)|招待状作成の一環として作成されたユーザー。読み取り専用|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

<!-- 
{ 
    "blockType": "resource",
    "keyProperty":"id",
    "@odata.type": "microsoft.graph.invitation", 
    "optionalProperties": [
        "invitedUser"
     ],
    "baseType": "microsoft.graph.entity"
} 
-->
```json
{
  "id": "string",
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
<!--
{
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
