---
title: oneNoteIdentity リソースの種類
description: '**まもなくサポートが提供される**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 0a7df80dd3dcd4f4b93edb4e708e65de3f74d775
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966448"
---
# <a name="onenoteidentity-resource-type"></a>oneNoteIdentity リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**まもなくサポートが提供される**

OneNoteIdentity 型は、_ユーザー_の id を表します。

今後、この型は[identity](identity.md)とマージされます。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|displayName|string|Id の表示名。|
|id|string|ID の一意識別子。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
