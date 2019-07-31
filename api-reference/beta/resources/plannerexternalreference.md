---
title: プラン/外部参照リソースの種類
description: '**Plan/externalreference**リソースは、参照 (ファイル、URL などの添付ファイル) のメタデータを表します。 これは、externalReferences オブジェクトのプロパティと値のペアの値です。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 2ac2b6bef3f2e4e24bfc6e789536f4952d89bb6d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966008"
---
# <a name="plannerexternalreference-resource-type"></a>プラン/外部参照リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Plan/externalreference**リソースは、参照 (ファイル、URL などの添付ファイル) のメタデータを表します。 これは、 [Externalreferences オブジェクト](plannerexternalreferences.md)のプロパティと値のペアの値です。



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|alias|String|参照を記述する名前のエイリアス。|
|lastModifiedBy|[identitySet](identityset.md)|読み取り専用です。 これを最後に変更するユーザー ID。|
|lastModifiedDateTime|DateTimeOffset|読み取り専用。 この時刻が最後に変更された日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|プレビューの優先度|String|タスクのプレビューとして参照が表示される相対的な優先順位を設定するために使用します。|
|type|String|参照の種類を記述するために使用します。 種類は`PowerPoint`、、 `Word`、 `Excel`、 `Other`です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
