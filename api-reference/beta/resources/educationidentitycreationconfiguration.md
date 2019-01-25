---
title: educationIdentityCreationConfiguration リソースの種類
description: 学校データ プロファイル id の作成時に設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリに作成されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 92ad3c36a9379bb570f2a635038903e64a0309e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511402"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a>educationIdentityCreationConfiguration リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

学校データ プロファイル id の作成時に設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリに作成されます。

> **注:** ディレクトリ同期がオンになって、設置型の間で同期する Active Directory と Azure Active Directory (AD の Azure) を使っている場合は、 [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)のリソースを使用してください。

[EducationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **userDomains** | [educationIdentityDomain](educationidentitydomain.md)コレクション |  ユーザーの種類ごとに使用するドメインの一覧を設定します。  |


## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitycreationconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
