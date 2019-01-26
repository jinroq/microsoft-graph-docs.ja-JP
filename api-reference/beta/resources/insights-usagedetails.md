---
title: usageDetails リソースの種類
description: 複合型を使用する項目のプロパティが含まれています。 リソースが最後にアクセスしたときに情報 (表示)、ユーザーが (編集) を変更します。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 04e064d5ebf8599466218722d89f46ececc5e58c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577488"
---
# <a name="usagedetails-resource-type"></a>usageDetails リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

複合型が[使用されている](insights-used.md)アイテムのプロパティが含まれています。 リソースが最後にアクセスしたときに情報 (表示)、ユーザーが (編集) を変更します。

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
| lastAccessedDateTime                  | DateTimeOffset        | 日付と時刻、リソースは、ユーザーが最後にアクセスしました。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z` 読み取り専用です。                      |
| lastModifiedDateTime              | DateTimeOffset        | 日付と時刻、ユーザーによってリソースが最後に修正されました。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z` 読み取り専用です。       |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-usagedetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
