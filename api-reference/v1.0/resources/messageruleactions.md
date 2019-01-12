---
title: messageRuleActions リソースの種類
description: ルールに使用可能なアクションのセットを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 33f1167d7317f941ebfa79b372e9cf575c14989b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914158"
---
# <a name="messageruleactions-resource-type"></a>messageRuleActions リソースの種類


ルールに使用可能なアクションのセットを表します。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| assignCategories | String コレクション | メッセージに割り当てられるカテゴリの一覧です。 |
| copyToFolder | String | メッセージのコピー先のフォルダーの ID です。 |
| delete | Boolean | 削除済みアイテム フォルダーにメッセージを移動する必要があるかどうかを示します。 |
| forwardAsAttachmentTo | [recipient](recipient.md) コレクション | 添付ファイルとしてメッセージを転送する受信者の電子メール アドレスです。 |
| forwardTo | [recipient](recipient.md) コレクション | メッセージを転送する受信者の電子メール アドレスです。 |
| markAsRead | Boolean | メッセージを開封済みにする必要があるかどうかを示します。 |
| markImportance | importance | メッセージの重要度を設定します。使用可能な値は、`low`、`normal`、`high` です。 |
| moveToFolder |  String| メッセージ移動先のフォルダーの ID です。 |
| permanentDelete | Boolean | メッセージを完全に削除し、削除済みアイテム フォルダーにメッセージを保存しないようにするかどうかを示します。 |
| redirectTo | [recipient](recipient.md) collection | メッセージのリダイレクト先の電子メール アドレス。 |
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
  "redirectTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
