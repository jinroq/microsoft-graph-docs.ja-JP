---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Quota
localization_priority: Normal
ms.openlocfilehash: a63b41253569dbb3d666a76b0a7495839ef61b12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882412"
---
# <a name="quota-resource-type"></a>クォータのリソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**クォータ**のリソースでは、容量に関する詳細情報を[ドライブ](drive.md)リソースの制約を提供します。

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

| プロパティ名 | Type   | 説明                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| total         | Int64  | 許可されている記憶域の合計 (バイト単位)。読み取り専用です。                           |
| used          | Int64  | 使用領域の合計 (バイト単位)。読み取り専用です。                                      |
| remaining     | Int64  | クォータ制限に達するまでの残りの領域の合計 (バイト単位)。読み取り専用です。 |
| deleted       | Int64  | ごみ箱内のファイルによって消費されている領域の合計 (バイト単位)。読み取り専用です。      |
| state         | 文字列 | 記憶域の状態を示す列挙値。読み取り専用です。 |
| storagePlanInformation  | [storagePlanInformation](storageplaninformation.md) | ドライブの記憶域のクォータの計画について説明します。 で個人の OneDrive です。|

### <a name="state-enumeration-values"></a>状態の列挙値

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
  "tocPath": "Facets/Quota"
} -->
