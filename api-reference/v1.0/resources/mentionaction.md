---
author: daspek
ms.author: dspektor
title: mentionAction リソースの種類
description: MentionAction オブジェクトは、活動中に説明されたユーザーに関する情報を提供します。
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 511519439f4079b2d7d618767855582f201c00f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036184"
---
# <a name="mentionaction-resource-type"></a>mentionAction リソースの種類

**MentionAction** リソースは、ユーザーについて記載した[アクティビティ][]に関する情報を提供します。

>**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。

[アクティビティ]: itemactivity.md

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類                       | 説明
|:--------------|:---------------------------|:-----------------------------
| mentionees    | [identitySet][] コレクション | このアクションに記載されているユーザーの ID。

[identitySet]: identityset.md

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction",
  "suppressions": []
}
-->
