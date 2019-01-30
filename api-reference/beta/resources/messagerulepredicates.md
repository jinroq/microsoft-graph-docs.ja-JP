---
title: messageRulePredicates リソースの種類
description: ルールで使用可能な条件および例外のセットを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fda6a160d30dc0d822f2e0aeb5642250d6b69658
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29644036"
---
# <a name="messagerulepredicates-resource-type"></a>messageRulePredicates リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ルールで使用可能な条件および例外のセットを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| bodyContains | コレクション (String) | 条件または例外を適用するために、受信メッセージの本文に表示される文字列を表します。 |
| bodyOrSubjectContains | コレクション (String) | 条件または例外を適用するために、受信メッセージの本文または件名に表示される文字列を表します。 |
| categories | コレクション (String) | 条件または例外を適用するために、受信メッセージにラベルを付けるカテゴリを表します。 |
| fromAddresses | コレクション ([Recipient](recipient.md)) | 条件または例外を適用するために、受信メッセージの特定の送信者のメール アドレスを表します。 |
| hasAttachments | Boolean | 条件または例外を適用するために、受信メッセージに添付ファイルがあるかどうかを示します。 |
| headerContains | コレクション (String) | 条件または例外を適用するために、受信メッセージのヘッダーに表示される文字列を表します。 |
| importance | String | 条件または例外を適用するために、受信メッセージに記録される重要性: `low`、`normal`、`high`。 |
| isApprovalRequest | Boolean | 条件または例外を適用するために、受信メッセージが承認要求であるかどうかを示します。 |
| isAutomaticForward | Boolean | 条件または例外を適用するために、受信メッセージが自動的に転送されるかどうかを示します。 |
| isAutomaticReply | Boolean | 条件または例外を適用するために、受信メッセージが自動返信であるかどうかを示します。 |
| isEncrypted | Boolean | 条件または例外を適用するために、受信メッセージが暗号化されるかどうかを示します。 |
| isMeetingRequest | Boolean | 条件または例外を適用するために、受信メッセージが会議出席依頼であるかどうかを示します。 |
| isMeetingResponse | Boolean | 条件または例外を適用するために、受信メッセージが会議出席依頼の返信であるかどうかを示します。 |
| isNonDeliveryReport | Boolean | 条件または例外を適用するために、受信メッセージが配信不能レポートであるかどうかを示します。 |
| IsPermissionControlled | Boolean | 条件または例外を適用するために、受信メッセージがアクセス許可制御 (RMS 保護) されるかどうかを示します。 |
| isReadReceipt | Boolean | 条件または例外を適用するために、受信メッセージが開封確認メッセージであるかどうかを示します。 |
| isSigned | Boolean | 条件または例外を適用するために、受信メッセージが S/MIME 署名されているかどうかを示します。 |
| isVoicemail | Boolean | 条件または例外を適用するために、受信メッセージがボイス メールかどうかを示します。 |
| messageActionFlag | String  | 条件または例外を適用するために、受信メッセージに表示されるアクション フラグの値を表します。 使用可能な値は、`any`、`call`、`doNotForward`、`followUp`、`fyi`、`forward`、`noResponseNecessary`、`read`、`reply`、`replyToAll`、`review` です。 |
| notSentToMe | Boolean | 条件または例外を適用するために、メールボックスの所有者が受信メッセージの受信者でないことを示します。 |
| recipientContains | コレクション (String) | 条件または例外を適用するために、受信メッセージの **ToRecipients** または **CcRecipients** プロパティに表示される文字列を表します。 |
| senderContains | コレクション (String) | 条件または例外を適用するために、受信メッセージの **From** プロパティに表示される文字列を表します。 |
| sensitivity | String | 条件または例外を適用するために、受信メッセージに記録される秘密度レベルを表します。使用可能な値: `normal`、`personal`、`private`、`confidential`。 |
| sentCcMe | Boolean | 条件または例外を適用するために、メールボックスの所有者が受信メッセージの **ccRecipients** プロパティにあるかどうかを示します。 |
| sentOnlyToMe | Boolean | 条件または例外を適用するために、メールボックスの所有者が受信メッセージの唯一の受信者かどうかを示します。 |
| sentToAddresses | コレクション ([Recipient](recipient.md)) | 条件または例外を適用するために、受信メッセージが送信されたメール アドレスを表します。 |
| sentToMe | Boolean | 条件または例外を適用するために、メールボックスの所有者が受信メッセージの **ToRecipients** プロパティにあるかどうかを示します。 |
| sentToOrCcMe | Boolean | 条件または例外を適用するために、メールボックスの所有者が受信メッセージの **toRecipients** または **ccRecipients** プロパティにあるかどうかを示します。 |
| subjectContains | コレクション (String) | 条件または例外を適用するために、受信メッセージの件名に表示される文字列を表します。 |
| withinSizeRange | [sizeRange](sizerange.md) | 条件または例外を適用するために、受信メッセージに想定される最小サイズと最大サイズ (単位: キロバイト) を表します。 |



## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRulePredicates"
}-->

```json
{
  "bodyContains": ["String"],
  "bodyOrSubjectContains": ["String"],
  "categories": ["String"],
  "fromAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": "Boolean",
  "headerContains": ["String"],
  "importance": "String",
  "isApprovalRequest": "Boolean",
  "isAutomaticForward": "Boolean",
  "isAutomaticReply": "Boolean",
  "isEncrypted": "Boolean",
  "isMeetingRequest": "Boolean",
  "isMeetingResponse": "Boolean",
  "isNonDeliveryReport": "Boolean",
  "isPermissionControlled": "Boolean",
  "isReadReceipt": "Boolean",
  "isSigned": "Boolean",
  "isVoicemail": "Boolean",
  "messageActionFlag": "String",
  "notSentToMe": "Boolean",
  "recipientContains": ["String"],
  "senderContains": ["String"],
  "sensitivity": "String",
  "sentCcMe": "Boolean",
  "sentOnlyToMe": "Boolean",
  "sentToAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "sentToMe": "Boolean",
  "sentToOrCcMe": "Boolean",
  "subjectContains": ["String"],
  "withinSizeRange": {"@odata.type": "microsoft.graph.sizeRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRulePredicates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/messagerulepredicates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
