---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
ms.openlocfilehash: 5e3b7cbf752d3ddb2c4b7bde3981d2a443028b92
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543248"
---
# <a name="deleteaction-resource-type"></a>DeleteAction リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[**itemActivity**][activity] に **DeleteAction** リソースがある場合、アクティビティがアイテムを削除したことを示します。

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類   | 説明
|:--------------|:-------|:----------------------------------------------------
| name          | string | 削除されたアイテムの名前。
| objectType    | string | `File`また`Folder`は、削除されたアイテムの種類によって異なります。

## <a name="remarks"></a>備考

アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。

<!--
{
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/deleteaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
