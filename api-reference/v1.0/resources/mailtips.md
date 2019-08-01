---
title: メールヒントリソースの種類
description: 'メッセージの作成中にユーザーに対して表示される、受信者に関する情報メッセージ。 たとえば、不在時のメッセージ '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 90f6f1a66631223a45a34797b6d18c13259d6241
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036324"
---
# <a name="mailtips-resource-type"></a>メールヒントリソースの種類

メッセージの作成中にユーザーに対して表示される、受信者に関する情報メッセージ。 たとえば、不在時のメッセージは、メッセージの受信者に対する自動応答として表示されます。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| 自動応答 | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | 受信者によって設定されている場合、自動応答のメールヒント。 |
| customMailTip | String | 受信者のメールボックスに設定できるカスタムメールヒント。 |
| deliveryRestricted| Boolean | 受信者のメールボックスが制限されているかどうか。たとえば、事前に定義された送信者の一覧からのメッセージの受信、送信者の定義済みリストからのメッセージの拒否、認証済みの送信者からのメッセージの受信のみを行います。 |
| emailAddress | [emailAddress](../resources/emailaddress.md) | メールヒントを取得する受信者の電子メールアドレス。 |
| error | [mailTipsError](../resources/mailtipserror.md) | [Getmailtips ヒント](../api/user-getmailtips.md)アクション中に発生するエラー。 |
| externalMemberCount | Int32 | 受信者が配布リストの場合の外部メンバーの数。 |
| isModerated |Boolean  | 受信者にメッセージを送信するには承認が必要であるかどうか。 たとえば、受信者が大きな配布リストであり、その配布リストに送信されたメッセージを承認するようにモデレーターが設定されている場合、または受信者にメッセージを送信する場合は、受信者の上司の承認が必要です。 |
| mailboxFull | Boolean | メールボックスのすべての受信者の状態。 |
| maxMessageSize | Int32 | 受信者の組織またはメールボックスに対して構成された最大メッセージサイズ。 |
| [受信者] スコープ | recipientScopeType | 受信者の範囲。 可能な値は、`none`、`internal`、`external`、`externalPartner`、`externalNonParther` です。 たとえば、管理者は別の組織を "パートナー" に設定することができます。 特定の範囲で特定のメールヒントにアクセスできるようにするには、スコープを使用すると便利です。 また、送信者に対して、メッセージが組織を離れていることを通知し、言葉、語調、およびコンテンツについての正しい判断を支援するためにも役立ちます。|
| 受信者候補 | [recipient](../resources/recipient.md) collection | 同じメッセージに表示される以前のコンテキストに基づいて提案される受信者。 |
| totalMemberCount | Int32 | 受信者が配布リストの場合のメンバー数。 |

### <a name="recipientscopetype-values"></a>recipientScopeType の値

| 値
|:-------------------------
| none
| 社外
| 社外
| externalPartner
| externalNonPartner


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
