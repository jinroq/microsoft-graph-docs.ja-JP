---
title: educationOneNoteResource リソースの種類
description: 'educationResource のサブクラス。 OneNote ページの場所を表します。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: a1d7796941edebe6ad1cb126d58b5e7600373ee0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340553"
---
# <a name="educationonenoteresource-resource-type"></a>educationOneNoteResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[educationResource](educationresource.md)のサブクラス。 OneNote ページの場所を表します。  

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|pageUrl|String|OneNote のページへの Microsoft Graph の URL。|
|sectionName|String|配布先のセクション名を指定します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
