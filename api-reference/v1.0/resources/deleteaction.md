---
author: daspek
ms.author: dspektor
title: deleteAction リソースの種類
description: DeleteAction オブジェクトは、アイテムの削除に関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 93f605e74a0a483a94593a9aaa40d6fd30efe914
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032733"
---
# <a name="deleteaction-resource-type"></a>deleteAction リソースの種類

[**Itemactivity**][activity]に**deleteaction**リソースが存在することは、アクティビティがアイテムを削除したことを示します。

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
