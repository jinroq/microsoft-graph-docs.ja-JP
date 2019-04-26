---
title: educationIdentityMatchingConfiguration リソースの種類
description: 学校データプロファイル id を照合するための設定を定義します。 これらの id には、学生と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリ内で更新されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0384fa269fd4304272d719df5860296d5f788c19
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340481"
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
