---
author: JeremyKelley
description: クォータリソースは、ドライブリソースの領域の制約に関する詳細を提供します。
ms.date: 09/10/2017
title: 領域
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 83e842872694a1f708bf37ab800fa73673255647
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008797"
---
# <a name="quota-resource-type"></a>クォータリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**クォータ**リソースは、[ドライブ](drive.md)リソースの領域の制約に関する詳細を提供します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "storagePlanInformation": {
    "upgradeAvailable": true
  },
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a>プロパティ

| プロパティ名 | 種類   | 説明                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| total         | Int64  | 許可されている記憶域の合計 (バイト単位)。読み取り専用です。                           |
| used          | Int64  | 使用領域の合計 (バイト単位)。読み取り専用です。                                      |
| remaining     | Int64  | クォータ制限に達するまでの残りの領域の合計 (バイト単位)。読み取り専用です。 |
| deleted       | Int64  | ごみ箱内のファイルによって消費されている領域の合計 (バイト単位)。読み取り専用です。      |
| state         | string | 記憶域の状態を示す列挙値。読み取り専用です。 |
| storagePlanInformation  | [storagePlanInformation](storageplaninformation.md) | ドライブの記憶域クォータプランに関する情報。 個人用の OneDrive のみ|

### <a name="state-enumeration-values"></a>状態列挙値

| 値      | 説明                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | ドライブに十分なクォータが残っています。                                                                                                                               |
| `nearing`  | 残りのクォータは、クォータ領域の合計の 10% 未満です。                                                                                                                      |
| `critical` | 残りのクォータは、クォータ領域の合計の 1% 未満です。                                                                                                                       |
| `exceeded` | クォータ使用量が、クォータの合計を超えています。クォータの合計を下回るか、追加の記憶領域を購入するまで、新しいファイルまたはフォルダーをドライブに追加することはできません。 |

<!--
{
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota",
  "suppressions": []
}
-->
