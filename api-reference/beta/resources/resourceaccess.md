---
title: resourceaccess リソースの種類
description: アプリケーションに必要な OAuth 2.0 アクセス許可スコープまたはアプリの役割を指定します。 requiredresourceaccess 型の**resourceaccess**プロパティは、 **resourceaccess**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: bb77a12a207e274b27263029d96f4ef260cfe5cb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343634"
---
# <a name="resourceaccess-resource-type"></a>resourceaccess リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションに必要な OAuth 2.0 アクセス許可スコープまたはアプリの役割を指定します。 [requiredresourceaccess](requiredresourceaccess.md)型の**resourceaccess**プロパティは、 **resourceaccess**のコレクションです。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|Guid|リソースアプリケーションが公開する[oAuth2Permission](oauth2permission.md)または[approle](approle.md)インスタンスの1つの一意識別子。|
|type|String|**id**プロパティが[oAuth2Permission](oauth2permission.md)または[approle](approle.md)のどちらを参照するかを指定します。 可能な値は、"scope" または "role" です。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
