---
title: educationCategory リソースの種類
description: 割り当てに適用できるカテゴリ。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bf5ee33ec7d217c0bc4c6e4d35666d6e9f34dadb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340602"
---
# <a name="educationcategory-resource-type"></a>educationCategory リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

割り当てに適用できるカテゴリ。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[educationCategory を取得する](../api/educationcategory-get.md) | [educationCategory](educationCategory.md) | 既存の**educationCategory**を取得します。|
|[カテゴリを削除する](../api/educationcategory-delete.md) | なし | **educationCategory**を削除します。|


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|String|カテゴリの一意識別子。|
|displayName|String|カテゴリの一意識別子。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCategory"
}-->

```json
{
  "id": "String (timestamp)",
  "displayName": "String (timestamp)",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationCategory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
