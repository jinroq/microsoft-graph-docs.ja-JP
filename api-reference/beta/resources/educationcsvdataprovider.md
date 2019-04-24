---
title: educationCsvDataProvider リソースの種類
description: 'CSV ファイルが入力ソースである場合に、学校データ同期プロファイルを設定するために使用されます。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bebacbc1c618c7558d81bde2611840e8d225a8fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507176"
---
# <a name="educationcsvdataprovider-resource-type"></a>educationCsvDataProvider リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

CSV ファイルが入力ソースである場合に、学校データ同期プロファイルを設定するために使用されます。  

[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **ユーザー** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 同期プロファイルに適用されるオプションのカスタマイズ。|

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationcsvdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
