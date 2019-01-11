---
title: educationIdentityDomain リソースの種類
description: '教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインのリソースは、ユーザー作成の構成の一部です。 '
localization_priority: Normal
ms.openlocfilehash: 5675499aca010f90deeb517210065ac4802d66b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807750"
---
# <a name="educationidentitydomain-resource-type"></a>educationIdentityDomain リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインのリソースは、[作成時の id の構成](educationidentitycreationconfiguration.md)の一部です。 

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **appliesTo** | 文字列 |  ライセンスを割り当てるにはユーザーのロールの種類です。 使用可能な値は、`student`、`teacher` です。      |
| **name** | 文字列 |  ユーザー アカウントのドメインを表します。         |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityDomain"
}-->

```json
{
    "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
    "name": "String"
}
```
