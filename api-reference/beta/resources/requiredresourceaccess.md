---
title: requiredResourceAccess リソースの種類
description: OAuth 2.0 のためのアクセス許可のスコープおよびアプリケーションへのアクセスを必要とする指定したリソース] の下のアプリケーション ロールのセットを指定します。 指定された OAuth 2.0 のアクセス許可の範囲を ( **requiredResourceAccess**コレクション) をクライアント アプリケーションで、要求することがリソースのアプリケーションを呼び出すことです。 アプリケーション エンティティの**requiredResourceAccess**プロパティは、 **ReqiredResourceAccess**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 473126365a7f0b3ba3ab0371322ff90bd36318e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856169"
---
# <a name="requiredresourceaccess-resource-type"></a>requiredResourceAccess リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|resourceAccess|[ResourceAccess](resourceaccess.md)コレクション|OAuth2.0 アクセス許可のスコープと、指定したリソースからアプリケーションを必要とするアプリケーション ロールの一覧です。|
|resourceAppId|String|アプリケーションへのアクセスに必要なリソースの一意の識別子です。  ターゲット リソースのアプリケーションで宣言されている**appId**に等しい場合があります。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
