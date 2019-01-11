---
title: educationIdentityMatchingOptions リソースの種類
description: ユーザー アカウントを一致させるためには、ソース プロパティとターゲット プロパティの間のマッピングを提供します。 元データ ソース プロパティが存在する必要があります。 ターゲット プロパティには、Azure Active Directory (AD の Azure) の有効なプロパティをする必要があります。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 80e9222f8f0c03294a947f403b33cc4f2cd2ef0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876280"
---
# <a name="educationidentitymatchingoptions-resource-type"></a>educationIdentityMatchingOptions リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ユーザー アカウントを一致させるためには、ソース プロパティとターゲット プロパティの間のマッピングを提供します。 元データ ソース プロパティが存在する必要があります。 ターゲット プロパティには、Azure Active Directory (AD の Azure) の有効なプロパティをする必要があります。

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **appliesTo** | 文字列 |  ライセンスを割り当てるにはユーザーのロールの種類です。 使用可能な値は、`student`、`teacher` です。      |
| **sourcePropertyName** | 文字列 |  ソース データ内のフィールド名をする必要があります、ソース プロパティの名前。 このプロパティは、大文字小文字を区別します。        |
| **targetPropertyName** | 文字列 |  Azure AD に有効なプロパティである必要がありますターゲット プロパティの名前です。 このプロパティは、大文字小文字を区別します。     |
| **targetDomain** | 文字列 |  ターゲット条件に一致するソース プロパティを使用して、サフィックスをドメイン。 として null を指定した場合、source プロパティを使用してターゲット プロパティと一致します。        |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingOptions"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "sourcePropertyName": "String",
    "targetPropertyName": "String",
    "targetDomain": "String"
}
```
