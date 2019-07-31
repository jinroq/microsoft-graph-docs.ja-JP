---
title: 共有リスト
description: ユーザーと共有されるファイルの一覧を返す、計算された洞察。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 5fa615e27f6fe1833af8d1b7c62c952623f5b703
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35953067"
---
# <a name="list-shared"></a>共有リスト

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーと共有されるファイルの一覧を返す、計算された洞察。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
```http
GET /me/insights/shared
```
' User id ' または ' userPrincipalName ' を持つ要求は、ユーザーのみがアクセスでき、他のユーザーはアクセスできません。
```http
GET /users/{id | userPrincipalName}/insights/shared
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

クエリパラメーターを使用`$filter`して、共有アイテムをフィルター処理できます。 たとえば、Type に基づいています。

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

利用可能なコンテナーの種類と種類を表示します。これは、 [Resourcevisualization](../resources/insights-resourcevisualization.md)でフィルター処理できます。

特定のユーザーによって共有されているファイルを取得することもできます。 たとえば、次のように`lastshared/sharedby/address`プロパティを指定します。

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

[Sharingdetail](../resources/insights-sharingdetail.md)複合型を参照してください。


## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       |  値|
|:-------------|:------|
| Authorization  | ベアラー {トークン}。必須。|
| 承諾  | application/json|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[共有](../resources/insights-shared.md)アイテムのリストを返します。
## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastShared" : { 
                "sharedDateTime" : "sharedDateTime-value",  
                "sharingSubject" : "sharingSubject-value",
                "sharingType" : "sharingType-value", 
                "sharedBy" : { 
                    "displayName" : "displayName-value", 
                    "id": "id-value" 
                }
                "sharingReference" : { 
                    "webUrl" : "webUrl-value",
                    "type: "type-value", 
                    "id": "id-value"
                } 
            },
            "resourceVisualization": { 
                "title" : "title-value, 
                "type"  : "type-value",
                "mediaType" : "mediaType-value",
                "previewImageUrl" : previewImageUrl-value, 
                "previewText" : "previewText-value", 
                "containerWebUrl" : "containerWebUrl-value", 
                "containerDisplayName" : "containerDisplayName-value", 
                "containerType" : "containerType-value" 
            }, 
            "resourceReference" : { 
                "webUrl" : "webUrl-value", 
                "id": "id-value", 
                "type: "type-value" 
}
```

### <a name="expanding-resource"></a>リソースの展開
共有された洞察で参照されているリソースは展開できます。
```http
GET https://graph.microsoft.com/beta/me/insights/shared/{id}/resource
```
