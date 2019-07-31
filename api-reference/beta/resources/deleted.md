---
author: JeremyKelley
description: Deleted リソースは、アイテムが削除されたことを示します。
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 2771f1c46fca5c352499dbfb3b41f718834da8b5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973128"
---
# <a name="deleted-facet"></a>Deleted ファセット

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**削除済み**リソースは、アイテムが削除されたことを示します。このバージョンの API では、リソースの値が存在する (null 以外である) ことは、ファイルが削除されたことを示します。null (または存在しない) 値は、ファイルが削除されていないことを示します。

変更の追跡と削除済みアイテムの検出の詳細については、「[アイテムの変更を表示する](../api/driveitem-delta.md)」を参照してください。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "state"
  ],
  "@odata.type": "microsoft.graph.deleted"
}-->
```json
{
  "state": "string"
}
```
## <a name="properties"></a>プロパティ

| プロパティ | 型   | 説明                               |
|:---------|:-------|:------------------------------------------|
| state    | String | 削除されたアイテムの状態を表します。 |

## <a name="remarks"></a>注釈 

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted",
  "suppressions": []
}
-->
