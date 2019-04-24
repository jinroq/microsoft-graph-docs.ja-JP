---
title: educationIdentityMatchingConfiguration リソースの種類
description: 学校データプロファイル id を照合するための設定を定義します。 これらの id には、学生と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリ内で更新されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: f8712cedf6cd8bd748b8bc29a17bea0779bbe253
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507119"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a>educationIdentityMatchingConfiguration リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

学校データプロファイル id を照合するための設定を定義します。 これらの id には、学生と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリ内で更新されます。

> **注:** このリソースが選択されている場合、ユーザーは作成されません。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **matchingOptions** | [educationIdentityMatchingOptions](educationidentitymatchingoptions.md)コレクション | ユーザーアカウントと、更新するユーザーを一意に識別するために使用するオプションとの間のマッピング。 |

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
