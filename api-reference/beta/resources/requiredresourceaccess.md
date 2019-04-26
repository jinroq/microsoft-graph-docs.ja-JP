---
title: requiredresourceaccess リソースの種類
description: アプリケーションがアクセスを必要とする、指定されたリソースの下にある OAuth 2.0 アクセス許可スコープおよびアプリロールのセットを指定します。 指定された OAuth 2.0 アクセス許可のスコープは、リソースアプリケーションを呼び出すときに、( **requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 application エンティティの**requiredresourceaccess**プロパティは、 **ReqiredResourceAccess**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: cd8049e7f843bbf057c79b4f3c90b7da51105191
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343669"
---
# <a name="requiredresourceaccess-resource-type"></a>requiredresourceaccess リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションがアクセスを必要とする、指定されたリソースの下にある OAuth 2.0 アクセス許可スコープおよびアプリロールのセットを指定します。 指定された OAuth 2.0 アクセス許可のスコープは、リソースアプリケーションを呼び出すときに、( **requiredresourceaccess**コレクションを通じて) クライアントアプリケーションによって要求されることがあります。 [application](application.md)エンティティの**requiredresourceaccess**プロパティは、 **ReqiredResourceAccess**のコレクションです。


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
|resourceAccess|[resourceaccess](resourceaccess.md)コレクション|指定されたリソースからアプリケーションが必要とする oauth 2.0 のアクセス許可スコープとアプリの役割の一覧。|
|resourceappid|String|アプリケーションがアクセスする必要があるリソースの一意識別子。  これは、ターゲットリソースアプリケーションで宣言されている**appId**と同じである必要があります。|

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
