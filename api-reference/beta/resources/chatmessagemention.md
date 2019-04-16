---
title: chatMessageMention リソースの種類
description: 'chatmessage エンティティ内のメンションを表します。 メンションは、ユーザー、チーム、ボット、またはチャネルにすることができます。 '
localization_priority: Normal
author: nkramer
ms.openlocfilehash: 5d7304325e48c87bfd75b57bf49585f66a77b262
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889997"
---
# <a name="chatmessagemention-resource-type"></a>chatMessageMention リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[chatmessage](chatmessage.md)エンティティ内のメンションを表します。 メンションは、ユーザー、チーム、ボット、またはチャネルにすることができます。 

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|int|記載されているエンティティのインデックス。 メッセージ本文の<at id="index">タグと一致します。|
|mentionText|string|メンションを表すために使用される文字列。 たとえば、ユーザーの表示名、チーム名などです。|
|明記|[identitySet](identityset.md)|前述したエンティティ (ユーザー、アプリケーション、チーム、またはチャネル)。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "number",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessagemention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
