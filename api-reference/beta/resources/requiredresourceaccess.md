---
title: requiredResourceAccess リソースの種類
description: アプリケーションがアクセスを必要とする、指定されたリソースの下にある OAuth 2.0 アクセス許可スコープおよびアプリロールのセットを指定します。 指定された OAuth 2.0 アクセス許可のスコープは、リソースアプリケーションを呼び出すときに、( **Requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 Application エンティティの**Requiredresourceaccess**プロパティは、 **ReqiredResourceAccess**のコレクションです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 6c7fec2027e5e987c66f868cc4a69555141bdbf9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965424"
---
# <a name="requiredresourceaccess-resource-type"></a>requiredResourceAccess リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションがアクセスを必要とする、指定されたリソースの下にある OAuth 2.0 アクセス許可スコープおよびアプリロールのセットを指定します。 指定された OAuth 2.0 アクセス許可のスコープは、リソースアプリケーションを呼び出すときに、( **Requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 [Application](application.md)エンティティの**requiredresourceaccess**プロパティは、 **ReqiredResourceAccess**のコレクションです。


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
|resourceAccess|[Resourceaccess](resourceaccess.md)コレクション|指定されたリソースからアプリケーションが必要とする OAuth 2.0 のアクセス許可スコープとアプリの役割の一覧。|
|resourceAppId|String|アプリケーションがアクセスする必要があるリソースの一意識別子。  これは、ターゲットリソースアプリケーションで宣言されている**appId**と同じである必要があります。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
