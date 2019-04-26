---
title: sharingdetail リソースの種類
description: '共有アイテムのプロパティを含む複合型。 '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 4a2dc75ed2a62d7a67538bdef801bd97133fbd15
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333565"
---
# <a name="sharingdetail-resource-type"></a>sharingdetail リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[共有](insights-shared.md)アイテムのプロパティを含む複合型。 

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingDetail"
}-->
```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a>プロパティ

| プロパティ              | 型          | 説明  |
| -------------         |-----------    | -------------|
| sharedDateTime        | DateTimeOffset| ファイルが最後に共有された日付と時刻。 Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z` 読み取り専用です。  |
| sharingsubject        | String          | ドキュメントが共有された件名。 |
| sharingtype             | String        | ドキュメントの共有方法を指定します。これは、"リンク"、"添付ファイル"、"グループ"、"Site" で指定できます。     |
| sharedBy                | [insightIdentity](insights-insightidentity.md)      | ドキュメントを共有したユーザー。  |
| sharingreference        | [resourceReference](insights-resourcereference.md)      |  |
