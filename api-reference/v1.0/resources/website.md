---
title: web サイトリソースの種類
description: Web サイトを表します。
localization_priority: Normal
ms.openlocfilehash: 1ffbee8a67527aac97bb4f60b7f8b1637ba1ebe5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457026"
---
# <a name="website-resource-type"></a>web サイトリソースの種類

Web サイトを表します。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|type|websiteType| 使用可能な値: `other`、`home`、`work`、`blog`、`profile`。|
|address|string|web サイトの URL。|
|displayName|string|Web サイトの表示名。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
