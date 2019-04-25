---
title: messageRuleActions リソースの種類
description: ルールに使用可能なアクションのセットを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a786a225bb9d439d60a29d2395b2d438975fc16c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523421"
---
# <a name="messageruleactions-resource-type"></a>messageRuleActions リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ルールに使用可能なアクションのセットを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| assignCategories | String コレクション | メッセージに割り当てられるカテゴリの一覧です。 |
| copyToFolder | String
 | メッセージのコピー先のフォルダーの ID です。 |
| delete | ブール型 | 削除済みアイテム フォルダーにメッセージを移動する必要があるかどうかを示します。 |
| forwardAsAttachmentTo | [recipient](recipient.md) collection | 添付ファイルとしてメッセージを転送する受信者の電子メール アドレスです。 |
| forwardTo | [recipient](recipient.md) コレクション | メッセージを転送する受信者の電子メール アドレスです。 |
| markAsRead | ブール型 | メッセージを開封済みにする必要があるかどうかを示します。 |
| markImportance | String
 | メッセージの重要度を設定します。使用可能な値は、`low`、`normal`、`high` です。 |
| moveToFolder |  String| メッセージ移動先のフォルダーの ID です。 |
| permanentDelete | ブール型 | メッセージを完全に削除し、削除済みアイテム フォルダーにメッセージを保存しないようにするかどうかを示します。 |
| redirectTo | [recipient](recipient.md) | メッセージのリダイレクト先の電子メール アドレスです。 |
| stopProcessingRules | Boolean | 後続のルールを評価する必要があるかどうかを示します。 |


## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": {"@odata.type": "microsoft.graph.recipient"},
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/messageruleactions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
