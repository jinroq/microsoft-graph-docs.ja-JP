---
title: educationPowerSchoolDataProvider リソース
description: PowerSchool は、入力ソースとして使用すると、学校のデータの同期プロファイルを設定するために使用します。
author: mmast-msft
ms.openlocfilehash: 714866d03c70aae8ea03a27b63fb3efbb4fa5ba4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312804"
---
# <a name="educationpowerschooldataprovider-resource"></a>educationPowerSchoolDataProvider リソース

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/)は、入力ソースとして使用すると、学校のデータの同期プロファイルを設定するために使用します。

[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。

## <a name="properties"></a>Properties

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **connectionUrl** | String | PowerSchool のインスタンスへの接続 URL です。 |
| **clientId** | String |  クライアント ID は、PowerSchool に接続するために使用します。 |
| **clientSecret** | String |  PowerSchool のインスタンスへの接続を認証するためにクライアントの機密情報です。 |
| **schoolsIds** | String コレクション |  学校の同期のリスト。 |
| **schoolYear** | String |  同期する学校の年です。 |
| **allowTeachersInMultipleSchools** | ブール型 |  ソースが 1 つの学生または教師の複数の識別子を持つかどうかを示します。 |
| **カスタマイズ** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | 同期プロファイルを適用するオプションのカスタマイズ。|

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
