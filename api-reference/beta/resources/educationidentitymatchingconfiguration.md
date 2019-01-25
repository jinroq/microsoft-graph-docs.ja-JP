---
title: educationIdentityMatchingConfiguration リソースの種類
description: 学校のデータのプロファイルの id を一致させるための設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリで更新されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f8712cedf6cd8bd748b8bc29a17bea0779bbe253
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520313"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a>educationIdentityMatchingConfiguration リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

学校のデータのプロファイルの id を一致させるための設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリで更新されます。

> **注:** このリソースが選択されている場合は、ユーザーは作成されません。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **matchingOptions** | [microsoft.graph.educationIdentityMatchingOptions](educationidentitymatchingoptions.md)コレクション | ユーザー アカウントを更新するユーザーを一意に識別に使用するオプションの間のマッピングです。 |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationidentitymatchingconfiguration.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
