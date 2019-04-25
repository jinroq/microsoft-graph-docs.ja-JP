---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: c951aa05b2b0f6f2b036bdf145e161a8d5b52ba7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544032"
---
# <a name="asyncjobstatus-resource"></a>AsyncJobStatus リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

このリソースは、非同期ジョブの進行状況に関する情報を提供します。

次の API 呼び出しは、**AsyncJobStatus** リソースを返します。

* [アイテムをコピーする](../api/driveitem-copy.md)

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a>プロパティ

| プロパティ名          | 種類   | 説明                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| **percentageComplete** | Double | 達成率を示す 0 〜 100 の値。                          |
| **status**             | String | ジョブの状態に関する有効な値の列挙にマップされる文字列値。 |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/resources/asyncjobstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
