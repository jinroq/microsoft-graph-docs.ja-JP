---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
ms.openlocfilehash: 68e6419206d03ba44cb34919ae46b8f1688d49a0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334634"
---
# <a name="editaction-resource-type"></a>EditAction リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[**itemActivity**][activity] に **EditAction** リソースがある場合、アクティビティがアイテムを編集したことを示します。

**注**:現在、このリソースは空ですが、将来のリビジョンでは、このリソースに追加のプロパティが設定される可能性があります。

[activity]: itemactivity.md

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
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
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction",
  "suppressions": []
}
-->
