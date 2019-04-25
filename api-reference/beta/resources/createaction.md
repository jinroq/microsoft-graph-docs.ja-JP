---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CreateAction
localization_priority: Normal
ms.openlocfilehash: 0872e74004fa65f1f1778c6e6123bb3c8af6c823
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543401"
---
# <a name="createaction-resource-type"></a>CreateAction リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[**itemActivity**][activity] に **CreateAction** リソースがある場合、アクティビティがアイテムを作成したことを示します。

**注**:現在、このリソースは空ですが、将来のリビジョンでは、このリソースに追加のプロパティが設定される可能性があります。

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.createAction"
}-->

```json
{
}
```

## <a name="properties"></a>プロパティ

なし。 このファセットは null 値または null 以外の値になり、プロパティは含まれていません。

## <a name="remarks"></a>備考

アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。

<!--
{
  "type": "#page.annotation",
  "description": "The CreateAction object provides information about the creation of an item.",
  "keywords": "activities,activity,action,create,creation",
  "section": "documentation",
  "tocPath": "Resources/CreateAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/createaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
