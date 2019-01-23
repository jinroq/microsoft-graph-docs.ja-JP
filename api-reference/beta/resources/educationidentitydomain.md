---
title: educationIdentityDomain リソースの種類
description: '教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインのリソースは、ユーザー作成の構成の一部です。 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 4eb9e5b58f62a23dbe1b450c2ec6b9d2f94970ac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395651"
---
# <a name="educationidentitydomain-resource-type"></a>educationIdentityDomain リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

教育のユーザーの種類とユーザーのアカウントが属するドメインとの間のマッピングを表します。 ドメインのリソースは、[作成時の id の構成](educationidentitycreationconfiguration.md)の一部です。 

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **appliesTo** | string |  ライセンスを割り当てるにはユーザーのロールの種類です。 使用可能な値は、`student`、`teacher` です。      |
| **name** | string |  ユーザー アカウントのドメインを表します。         |

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
