---
title: resourceaccess リソースの種類
description: アプリケーションに必要な OAuth 2.0 アクセス許可スコープまたはアプリの役割を指定します。 requiredresourceaccess 型の**resourceaccess**プロパティは、 **resourceaccess**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 1e741aa49e56b304c265a5fd701fdac37feb29dd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563056"
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
