---
title: educationIdentityDomain リソースの種類
description: '教育ユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインリソースは、id 作成構成の一部です。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5cf7444c51b34ae4a8eacf9c99fdfd085dbec896
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334269"
---
# <a name="educationidentitydomain-resource-type"></a>educationIdentityDomain リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

教育ユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインリソースは、 [id 作成構成](educationidentitycreationconfiguration.md)の一部です。 

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **appliesTo** | string |  ライセンスに割り当てるユーザーの役割の種類。 可能な値は、`student`、`teacher` です。      |
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
