---
title: リストの使用
description: ユーザーに使用されるファイルの一覧を返す計算の把握。
ms.openlocfilehash: a9e5390e38e4e697f55676304edb4544e4c2ded5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070946"
---
# <a name="list-used"></a>リストの使用

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ユーザーに使用されるファイルの一覧を返す計算の把握。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Sites.Read.All、Sites.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Sites.Read.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
```http
GET /me/insights/used
```
'LastModifiedDateTime' で並べ替えられた結果が返されます他のユーザーのドキュメントの使用を要求して、'lastAccessedDateTime' は、'lastModifiedDateTime' に設定されています。
```http
GET /users/<id | userPrincipalName>/insights/used
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

使用することができます、`$filter`アイテムのフィルターを使用するパラメーター クエリを実行します。 などは、型に基づいています。

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/Type eq 'PowerPoint'`

コンテナーの種類に基づくか。

`https://graph.microsoft.com/beta/me/insights/used?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

使用可能なコンテナーの種類と[resourceVisualization](../resources/insights-resourcevisualization.md)内でフィルターの種類を参照してください。


## <a name="request-headers"></a>要求ヘッダー
| ヘッダー       |  値|
|:-------------|:------|
| Authorization  | ベアラー {トークン}。必須。|
| 承諾  | application/json|

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本体で[使用する](../resources/insights-used.md)項目の一覧です。
## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。
```http
GET https://graph.microsoft.com/beta/me/insights/used
```

##### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。 
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastused" : { 
                "lastAccessedDateTime" : "lastAccessedDateTime-value", 
                "lastModifiedDateTime": "lastModifiedDateTime-value" 
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
        }
    ]
}
```

### <a name="expanding-resource"></a>リソースを展開します。
使用の洞察によって参照されるリソースを展開します。
```http
GET https://graph.microsoft.com/beta/me/insights/used/{id}/resource
```