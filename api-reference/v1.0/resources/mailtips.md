---
title: リソースの種類のメール ヒント
description: 'メッセージの作成中にユーザーに表示される、受信者に関する情報メッセージです。 たとえば、不在時のメッセージ '
localization_priority: Normal
ms.openlocfilehash: 0506d10ad4b1c5eb473b04a30eb8d48334685574
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891694"
---
# <a name="mailtips-resource-type"></a>リソースの種類のメール ヒント

メッセージの作成中にユーザーに表示される、受信者に関する情報メッセージです。 など、不在時のメッセージ、自動返信メッセージの受信者として。


## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | 受信者によって設定されている場合の自動応答に関するメールのヒント。 |
| customMailTip | String | 受信者のメールボックスに設定可能なカスタム メールのヒント。 |
| deliveryRestricted| Boolean | 受信者のメールボックスが制限されているかどうか。たとえば、送信者の定義済みリストからのメッセージのみを受け付ける、送信者の定義済みリストからのメッセージを拒否する、または認証された送信者からのメッセージのみを受信するなどです。 |
| emailAddress | [emailAddress](../resources/emailaddress.md) | メールヒントを取得する受信者の電子メール アドレス。 |
| エラー | [mailTipsError](../resources/mailtipserror.md) | [GetMailTips](../api/user-getmailtips.md)操作中に発生するエラーです。 |
| externalMemberCount | Int32 | 受信者が配布リストの場合は外部メンバーの数です。 |
| isModerated |Boolean  | 受信者へのメッセージ送信に承認が必要かどうか。たとえば、受信者が大規模な配布リストであり、モデレーターが配布リストに送信されたメッセージを承認するようにセットアップされている場合、または受信者へのメッセージの送信に受信者の上司の承認を必要とする場合などです。 |
| mailboxFull | Boolean | 受信者のメールボックスのフル状態。 |
| maxMessageSize | Int32 | 受信者の組織またはメールボックスに対して構成されているメッセージの最大サイズ。 |
| recipientScope | recipientScopeType | 受信者のスコープ。 可能な値は、`none`、`internal`、`external`、`externalPartner`、`externalNonParther` です。 たとえば、管理者は、その「パートナー」になるように別の組織を設定できます。 スコープは、管理者が特定のスコープにアクセスできるようにする特定のメール ヒントを希望する場合に便利です。 送信者のメッセージが言葉使い、トーン、およびコンテンツに関する正しい判断を下すことを支援、組織になることを通知するに有用なもあります。|
| recipientSuggestions | [recipient](../resources/recipient.md) collection | 同じメッセージに表示される前のコンテキストに基づいて提案される受信者。 |
| totalMemberCount | Int32 | 受信者が配布リストの場合はメンバー数です。 |

### <a name="recipientscopetype-values"></a>recipientScopeType 値

| 値
|:-------------------------
| none
| 内部
| 外部
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
