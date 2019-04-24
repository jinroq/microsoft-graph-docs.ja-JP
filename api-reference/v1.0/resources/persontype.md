---
title: personType リソースの種類
description: 個人の種類を表します。
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 270fa800242ae7a25ed0f5959a97b6a70f7cedd3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462460"
---
# <a name="persontype-resource-type"></a>personType リソースの種類

個人の種類を表します。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personType"
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|クラス|String|データ ソースの種類 (Person など)。|
|サブクラス|String|データ ソースの 2 番目の種類 (OrganizationUser など)。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
