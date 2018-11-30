---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
ms.openlocfilehash: 4319ab0f36e12ddd28ca9bb6c7bfd48043228504
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067518"
---
# <a name="incompletedata-resource-type"></a>incompleteData リソースの種類

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**IncompleteData**ファセットは、不完全なデータとリソースが生成されたことを示します。
内でプロパティがについての情報を提供するには、不完全なデータがある理由です。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a>プロパティ

| プロパティ                  | 型           | 説明
|:--------------------------|:---------------|:--------------------------------
| missingDataBeforeDateTime | DateTimeOffset | サービスには、指定された時間の前にソース データがありません。
| wasThrottled              | ブール値        | データの一部は、過剰な活動のため録画されませんでした。

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData"
} -->
