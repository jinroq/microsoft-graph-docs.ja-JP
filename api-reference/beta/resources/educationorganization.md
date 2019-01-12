---
title: educationOrganization リソースの種類
description: '教育セクター内の別の組織の種類との間の共通性をモデル化するために使用する抽象エンティティです。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a1e3f82e2d777b1d32cc445f543e7beed570a8b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949522"
---
# <a name="educationorganization-resource-type"></a>educationOrganization リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

教育セクター内の別の組織の種類との間の共通性をモデル化するために使用する抽象エンティティです。  

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|説明|String| 組織の説明です。|
|displayName|String| 組織の表示名です。|
|externalSource|文字列| この組織が作成されたソースです。 可能な値は、`sis`、`manual`、`unknownFutureValue` です。|

## <a name="relationships"></a>リレーションシップ
なし。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
