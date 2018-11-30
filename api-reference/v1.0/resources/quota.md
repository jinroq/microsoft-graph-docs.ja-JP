---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Quota
ms.openlocfilehash: 54eb88bdc048c6b63bb6f2d0a23fb05023663ca7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021217"
---
# <a name="quota-resource-type"></a>クォータ リソースの種類

**クォータ** リソースは、[ドライブ](drive.md) リソースの領域の制約に関する詳細を提供します。

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

## <a name="state-enumeration"></a>状態の列挙値

| 値      | 説明                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | ドライブに十分なクォータが残っています。                                                                                                                               |
| `nearing`  | 残りのクォータは、クォータ領域の合計の 10% 未満です。                                                                                                                      |
| `critical` | 残りのクォータは、クォータ領域の合計の 1% 未満です。                                                                                                                       |
| `exceeded` | クォータ使用量が、クォータの合計を超えています。クォータの合計を下回るか、追加の記憶領域を購入するまで、新しいファイルまたはフォルダーをドライブに追加することはできません。 |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/quota.md:
      Found potential enums in resource example that weren't defined in a table:(normal, nearing,critical,exceeded) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Quota"
} -->
