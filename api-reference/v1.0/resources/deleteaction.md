---
author: daspek
ms.author: dspektor
title: deleteAction リソースの種類
description: DeleteAction オブジェクトは、アイテムの削除に関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ba5004c17f1cc71f66420a81b5eb66603df00eee
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970779"
---
# <a name="deleteaction-resource-type"></a>deleteAction リソースの種類

[**Itemactivity**] [ activity]に**deleteaction**リソースが存在することは、アクティビティがアイテムを削除したことを示します。

>**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。

[activity]: itemactivity.md

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類   | 説明
|:--------------|:-------|:----------------------------------------------------
| name          | string | 削除されたアイテムの名前。
| objectType    | string | `File`また`Folder`は、削除されたアイテムの種類によって異なります。


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

<!--
{
  "type": "#page.annotation",
  "description": "The deleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
