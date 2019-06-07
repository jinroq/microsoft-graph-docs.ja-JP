---
title: educationIdentityMatchingOptions リソースの種類
description: ソースプロパティと、一致するユーザーアカウントのターゲットプロパティとの間のマッピングを提供します。 Source プロパティはソースデータに存在する必要があります。 Target プロパティは、Azure Active Directory (Azure AD) の有効なプロパティである必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 37ebb55fdd5457841ca0083c18518babca7565c4
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750151"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>educationIdentityMatchingOptions リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ソースプロパティと、一致するユーザーアカウントのターゲットプロパティとの間のマッピングを提供します。 Source プロパティはソースデータに存在する必要があります。 Target プロパティは、Azure Active Directory (Azure AD) の有効なプロパティである必要があります。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **appliesTo** | string |  ライセンスに割り当てるユーザーロールの種類。 可能な値は、`student`、`teacher`、`faculty` です。      |
| **sourcePropertyName** | string |  Source プロパティの名前です。ソースデータのフィールド名を指定する必要があります。 このプロパティは大文字と小文字を区別します。        |
| **targetPropertyName** | string |  ターゲットプロパティの名前。これは、Azure AD の有効なプロパティである必要があります。 このプロパティは大文字と小文字を区別します。     |
| **targetDomain** | string |  ターゲットに一致する source プロパティを持つ、ドメインのサフィックス。 Null として指定された場合、source プロパティを使用してターゲットプロパティと照合します。        |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
