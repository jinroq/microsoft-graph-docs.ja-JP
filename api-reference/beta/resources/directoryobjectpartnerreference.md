---
title: directoryObjectPartnerReference リソースの種類
description: パートナー テナント内のディレクトリ オブジェクトへの参照を表します。 directoryObject から継承します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a031586d1f92bf2b8b331e9b71058211b4617382
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640309"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>directoryObjectPartnerReference リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

パートナー組織内のディレクトリ オブジェクトへの参照を表します。 [directoryObject](directoryobject.md?view=graph-rest-beta) から継承します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|説明|String| オブジェクトの説明が返されます。 読み取り専用です。 |
|displayName|String| グループまたはアプリケーションのように、返されるディレクトリ オブジェクトの名前です。 読み取り専用です。 |
|externalPartnerTenantId|Guid| パートナー テナントにテナントの識別子です。 読み取り専用です。 |
|id|String| リソースの一意識別子。 [directoryObject](directoryobject.md?view=graph-rest-beta) から継承されます。 読み取り専用です。 |
|objectType|String| パートナー テナントで参照されるオブジェクトの型。 読み取り専用です。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}-->

```json
{
  "description": "string ",
  "displayName": "string",
  "externalPartnerTenantId": "string (identifier)",
  "id": "string (identifier)",
  "objectType": "string"
}
```

## <a name="see-also"></a>関連項目

- [ID のリストからディレクトリ オブジェクトを取得します。](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryobjectpartnerreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
