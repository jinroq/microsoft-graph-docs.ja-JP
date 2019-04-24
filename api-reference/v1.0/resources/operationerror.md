---
title: operationerror リソースの種類
description: teamsAsyncOperation のエラーについて説明します。
localization_priority: Normal
ms.openlocfilehash: 22590d7d955cf01385292d2796ad960b1c0ced41
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462607"
---
# <a name="operationerror-resource-type"></a>operationerror リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[teamsAsyncOperation](teamsasyncoperation.md)のエラーについて説明します。

## <a name="operationerror-properties"></a>operationerror プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|code|string (読み取り専用)|操作エラーコード。|
|message|string (読み取り専用)|操作エラーメッセージ。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/operationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
