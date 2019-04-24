---
title: educationCategory リソースの種類
description: 割り当てに適用できるカテゴリ。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 928f37b4d29a4443c947bd92bf4a71f9f8a05f59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507318"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationcategory.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
