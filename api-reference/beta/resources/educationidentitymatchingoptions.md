---
title: educationIdentityMatchingOptions リソースの種類
description: ソースプロパティと、一致するユーザーアカウントのターゲットプロパティとの間のマッピングを提供します。 source プロパティはソースデータに存在する必要があります。 target プロパティは、azure Active Directory (azure AD) の有効なプロパティである必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7ce68460e8dfd0ff3e58b51d0007278aa6c9426e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334243"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>educationIdentityMatchingOptions リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ソースプロパティと、一致するユーザーアカウントのターゲットプロパティとの間のマッピングを提供します。 source プロパティはソースデータに存在する必要があります。 target プロパティは、azure Active Directory (azure AD) の有効なプロパティである必要があります。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **appliesTo** | string |  ライセンスに割り当てるユーザーロールの種類。 可能な値は、`student`、`teacher` です。      |
| **sourcepropertyname** | string |  source プロパティの名前です。ソースデータのフィールド名を指定する必要があります。 このプロパティは大文字と小文字を区別します。        |
| **targetpropertyname** | string |  ターゲットプロパティの名前。これは、Azure AD の有効なプロパティである必要があります。 このプロパティは大文字と小文字を区別します。     |
| **targetdomain** | string |  ターゲットに一致する source プロパティを持つ、ドメインのサフィックス。 null として指定された場合、source プロパティを使用してターゲットプロパティと照合します。        |

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
