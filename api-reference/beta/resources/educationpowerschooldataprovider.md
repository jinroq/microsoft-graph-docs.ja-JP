---
title: educationPowerSchoolDataProvider リソース
description: powerschool が入力ソースとして使用されている場合に、学校データ同期プロファイルを設定するために使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2469a99b8acbfa1bd4e5167cf67caa102fa9422e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507127"
---
# <a name="educationpowerschooldataprovider-resource"></a>educationPowerSchoolDataProvider リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[powerschool](https://www.powerschool.com/solutions/student-information-system-sis/)が入力ソースとして使用されている場合に、学校データ同期プロファイルを設定するために使用されます。

[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **connectionurl** | String | powerschool インスタンスへの接続 URL。 |
| **clientId** | String |  powerschool への接続に使用されるクライアント ID。 |
| **clientSecret** | String |  powerschool インスタンスへの接続を認証するクライアントシークレット。 |
| **schoolsIds** | String collection |  同期する教育機関のリスト。 |
| **schoolYear** | String |  同期する学校の年。 |
| **allowTeachersInMultipleSchools** | Boolean |  単一の学生または教師に対して、ソースに複数の識別子があるかどうかを示します。 |
| **ユーザー** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 同期プロファイルに適用されるカスタマイズ (オプション)。|

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerschooldataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
