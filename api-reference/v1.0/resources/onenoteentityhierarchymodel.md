---
title: onenoteEntityHierarchyModel リソース
description: これは、OneNote のエンティティの基本型です。
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 9dbab25bb3afa69c434545fceaa6cbc869fb7dcc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858878"
---
# <a name="onenoteentityhierarchymodel-resource"></a>onenoteEntityHierarchyModel リソース

これは、OneNote のエンティティの基本型です。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityHierarchyModel"
}-->

```json
{
  "displayName": "string",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a>プロパティ
## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|displayName|String|ノートブックの名前。|
|createdBy|[identitySet](identityset.md)|そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。|
|lastModifiedBy|[identitySet](identityset.md)|そのアイテムを作成したユーザーの ID、デバイス、アプリケーション。読み取り専用です。|
|lastModifiedDateTime|DateTimeOffset|ノートブックが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。|

<!-- uuid: 8b1af557-1a7c-4432-86eb-94989c2d4b54
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
