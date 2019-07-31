---
title: insightIdentity
description: 共有アイテムのプロパティを含む複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 6b5a4b3c6e43f0314860935af810d20d91663c96
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005752"
---
# <a name="insightidentity"></a>insightIdentity

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[共有](insights-shared.md)アイテムのプロパティを含む複合型。 

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.insightIdentity"
}-->
```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ              | 型          | 説明  |
| -------------         |-----------    | -------------|
| displayName       | String          | アイテムを共有したユーザーの表示名。 |
| id              | 文字列        | アイテムを共有したユーザーの id。     |
| address             | String      | アイテムを共有したユーザーの電子メールアドレス。  |
