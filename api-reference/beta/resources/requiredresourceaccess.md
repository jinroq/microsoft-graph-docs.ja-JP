---
title: requiredResourceAccess リソースの種類
description: OAuth 2.0 のためのアクセス許可のスコープおよびアプリケーションへのアクセスを必要とする指定したリソース] の下のアプリケーション ロールのセットを指定します。 指定された OAuth 2.0 のアクセス許可の範囲を ( **requiredResourceAccess**コレクション) をクライアント アプリケーションで、要求することがリソースのアプリケーションを呼び出すことです。 アプリケーション エンティティの**requiredResourceAccess**プロパティは、 **ReqiredResourceAccess**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: a2c7e337bbe441275f395c2333b8cee918e6b9da
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512970"
---
# <a name="requiredresourceaccess-resource-type"></a>requiredResourceAccess リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OAuth 2.0 のためのアクセス許可のスコープおよびアプリケーションへのアクセスを必要とする指定したリソース] の下のアプリケーション ロールのセットを指定します。 指定された OAuth 2.0 のアクセス許可の範囲を ( **requiredResourceAccess**コレクション) をクライアント アプリケーションで、要求することがリソースのアプリケーションを呼び出すことです。 [アプリケーション](application.md)エンティティの**requiredResourceAccess**プロパティは、 **ReqiredResourceAccess**のコレクションです。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|resourceAccess|[ResourceAccess](resourceaccess.md)コレクション|OAuth2.0 アクセス許可のスコープと、指定したリソースからアプリケーションを必要とするアプリケーション ロールの一覧です。|
|resourceAppId|String|アプリケーションへのアクセスに必要なリソースの一意の識別子です。  ターゲット リソースのアプリケーションで宣言されている**appId**に等しい場合があります。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/requiredresourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
