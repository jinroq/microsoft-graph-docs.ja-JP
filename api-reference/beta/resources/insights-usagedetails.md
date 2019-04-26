---
title: 種類の詳細リソースの種類
description: 使用されているアイテムのプロパティを含む複合型。 ユーザーによってリソースが最後にアクセス (表示) され、変更 (編集) された日時に関する情報。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: d8a8893f2c5fcb21e2e578eefa4cf5733782db07
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333534"
---
# <a name="usagedetails-resource-type"></a>種類の詳細リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[使用され](insights-used.md)ているアイテムのプロパティを含む複合型。 ユーザーによってリソースが最後にアクセス (表示) され、変更 (編集) された日時に関する情報。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usageDetails"
}-->

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a>プロパティ

| プロパティ              | 型          | 説明  |
| -------------         |---------------| -------------|
| lastAccessedDateTime                  | DateTimeOffset        | リソースが最後にユーザーによってアクセスされた日付と時刻。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z` 読み取り専用です。                      |
| lastModifiedDateTime              | DateTimeOffset        | ユーザーによってリソースが最後に変更された日付と時刻。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z` 読み取り専用です。       |
