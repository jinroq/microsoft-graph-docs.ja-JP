---
title: resourceAccess リソースの種類
description: アプリケーションに必要な OAuth 2.0 アクセス許可スコープまたはアプリの役割を指定します。 RequiredResourceAccess 型の**resourceaccess**プロパティは、 **resourceaccess**のコレクションです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4c2a909fb2beafeb22f303ef42703b3d57c30854
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965414"
---
# <a name="resourceaccess-resource-type"></a>resourceAccess リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションに必要な OAuth 2.0 アクセス許可スコープまたはアプリの役割を指定します。 [Requiredresourceaccess](requiredresourceaccess.md)型の**resourceaccess**プロパティは、 **resourceaccess**のコレクションです。


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
|type|String|**Id**プロパティが[OAuth2Permission](oauth2permission.md)または[approle](approle.md)のどちらを参照するかを指定します。 可能な値は、"scope" または "role" です。|

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
