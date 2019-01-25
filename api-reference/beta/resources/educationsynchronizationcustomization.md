---
title: educationSynchronizationCustomization リソースの種類
description: 'リソース エンティティの学校データ プロファイルの同期をカスタマイズするための設定を提供します。 同期されているすべてのエンティティには、カスタマイズを適用できます。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513607"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>educationSynchronizationCustomization リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

リソース エンティティの学校データ プロファイルの同期をカスタマイズするための設定を提供します。 同期されているすべてのエンティティには、カスタマイズを適用できます。 

>**注:****SynchronizationStartDate**プロパティは、 **StudentEnrollment**のエンティティにのみ適用されます。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **optionalPropertiesToSync** | Collection of String |  同期するプロパティ名のコレクションです。かどうかのセットを null に、すべてのプロパティが同期します。       |
| **synchronizationStartDate** | DateTime
 |  同期を開始する日付。 この値は、将来の日付に設定する必要があります。 場合は null の場合、リソースに設定は、プロファイルの設定が完了したときに同期されます。 **注:** これは、 **StudentEnrollment**プロパティにのみ適用されます。      |
|**isSyncDeferred** |ブール値 | 親エンティティの同期がそれ以降の日付に延期されたかどうかを示します。 |
| **allowDisplayNameUpdate** | ブール値 |  同期によって、リソースの表示名を上書きするかどうかを示します。         |


## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
