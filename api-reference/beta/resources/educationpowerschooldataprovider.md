---
title: educationPowerSchoolDataProvider リソース
description: powerschool が入力ソースとして使用されている場合に、学校データ同期プロファイルを設定するために使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: cee763995dd5a75b64d94e5f170d6fea992c20b5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340575"
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
  "schoolsIds": ["String"],
  "schoolYear": "String",
  "allowTeachersInMultipleSchools": "Boolean",
  "customizations": {"@odata.type": "microsoft.graph.educationSynchronizationCustomizations"}
}
```
