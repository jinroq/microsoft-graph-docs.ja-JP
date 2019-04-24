---
title: educationSynchronizationCustomization リソースの種類
description: 'リソースエンティティの学校データプロファイルの同期をカスタマイズするための設定を提供します。 カスタマイズは、同期対象のすべてのエンティティに適用できます。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507050"
---
# <a name="educationsynchronizationcustomization-resource-type"></a>educationSynchronizationCustomization リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

リソースエンティティの学校データプロファイルの同期をカスタマイズするための設定を提供します。 カスタマイズは、同期対象のすべてのエンティティに適用できます。 

>**注:****同期**開始プロパティは、 **StudentEnrollment**エンティティにのみ適用されます。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **optionalPropertiesToSync** | 文字列のコレクション |  同期するプロパティ名のコレクション。null に設定されている場合、すべてのプロパティが同期されます。       |
| **同期開始日** | DateTime
 |  同期を開始する日付を指定します。 この値は、将来の日付に設定する必要があります。 null に設定されている場合、プロファイルの設定が完了すると、リソースが同期されます。 **注:** これは、 **StudentEnrollment**プロパティにのみ適用されます。      |
|**issyncdeferred** |Boolean | 親エンティティの同期を後日延期するかどうかを示します。 |
| **allowdisplaynameupdate** | Boolean |  同期によってリソースの表示名を上書きできるかどうかを示します。         |


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
