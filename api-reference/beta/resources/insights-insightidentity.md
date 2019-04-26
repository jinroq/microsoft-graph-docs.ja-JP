---
title: insightIdentity
description: 共有アイテムのプロパティを含む複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 8718ab248dada75f04d92d6a8717dd4f43ee8106
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333597"
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
| id              | String        | アイテムを共有したユーザーの id。     |
| address             | String      | アイテムを共有したユーザーの電子メールアドレス。  |
