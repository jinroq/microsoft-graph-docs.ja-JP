---
title: educationIdentityDomain リソースの種類
description: '教育ユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインリソースは、id 作成構成の一部です。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 628fbdea770c685eca0194fb95a314e2e542d2fc
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34750158"
---
# <a name="educationidentitydomain-resource-type"></a>educationIdentityDomain リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

教育ユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインリソースは、 [id 作成構成](educationidentitycreationconfiguration.md)の一部です。 

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **appliesTo** | string |  ライセンスに割り当てるユーザーロールの種類。 可能な値は、`student`、`teacher`、`faculty` です。      |
| **name** | string |  ユーザーアカウントのドメインを表します。         |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "microsoft.graph.educationUserRole"},
    "name": "String"
}
```
