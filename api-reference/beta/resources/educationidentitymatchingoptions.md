---
title: educationIdentityMatchingOptions リソースの種類
description: ユーザー アカウントを一致させるためには、ソース プロパティとターゲット プロパティの間のマッピングを提供します。 元データ ソース プロパティが存在する必要があります。 ターゲット プロパティには、Azure Active Directory (AD の Azure) の有効なプロパティをする必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: c2b092d5589cdccccfe73a7e71afcafa7b555a90
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425793"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>educationIdentityMatchingOptions リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

ユーザー アカウントを一致させるためには、ソース プロパティとターゲット プロパティの間のマッピングを提供します。 元データ ソース プロパティが存在する必要があります。 ターゲット プロパティには、Azure Active Directory (AD の Azure) の有効なプロパティをする必要があります。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **appliesTo** | string |  ライセンスを割り当てるにはユーザーのロールの種類です。 使用可能な値は、`student`、`teacher` です。      |
| **sourcePropertyName** | string |  ソース データ内のフィールド名をする必要があります、ソース プロパティの名前。 このプロパティは、大文字小文字を区別します。        |
| **targetPropertyName** | string |  Azure AD に有効なプロパティである必要がありますターゲット プロパティの名前です。 このプロパティは、大文字小文字を区別します。     |
| **targetDomain** | string |  ターゲット条件に一致するソース プロパティを使用して、サフィックスをドメイン。 として null を指定した場合、source プロパティを使用してターゲット プロパティと一致します。        |

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
