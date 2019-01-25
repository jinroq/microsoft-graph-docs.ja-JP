---
title: resourceAccess リソースの種類
description: OAuth 2.0 のためのアクセス許可のスコープまたはアプリケーションを必要とするアプリケーションの役割を指定します。 RequiredResourceAccess 型の**resourceAccess**プロパティは、 **ResourceAccess**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 1e741aa49e56b304c265a5fd701fdac37feb29dd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519025"
---
# <a name="resourceaccess-resource-type"></a>resourceAccess リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OAuth 2.0 のためのアクセス許可のスコープまたはアプリケーションを必要とするアプリケーションの役割を指定します。 [RequiredResourceAccess](requiredresourceaccess.md)型の**resourceAccess**プロパティは、 **ResourceAccess**のコレクションです。


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
|ID|Guid|リソースのアプリケーションを公開する[oAuth2Permission](oauth2permission.md)または[エンティティ](approle.md)のインスタンスの 1 つの一意の識別子です。|
|type|String|[OAuth2Permission](oauth2permission.md)または[エンティティ](approle.md)の**id**プロパティを参照するかどうかを指定します。 使用可能な値は、「スコープ」または「ロール」です。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
