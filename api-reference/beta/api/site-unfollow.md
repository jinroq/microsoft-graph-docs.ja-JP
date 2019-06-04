---
author: learafa
title: フォロー取り消しサイト
description: ユーザーのサイトのフォローを取り消します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 63027ab1fcf47baaf8709db1c5c22089e0dbb7a9
ms.sourcegitcommit: 895a03cb2706a9b3a2236b30d6a7e9f5cbc6a89e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2019
ms.locfileid: "34692795"
---
# <a name="unfollow-site"></a>フォロー取り消しサイト 

ユーザーの[サイト](../resources/site.md)または複数のサイトのフォローを取り消します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|            アクセス許可の種類             | アクセス許可 (特権の小さいものから大きいものへ) |
| :------------------------------------- | :------------------------------------------ |
| 委任 (職場または学校のアカウント)     | Sites.ReadWrite.All                         |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                              |
| アプリケーション                            | Sites.ReadWrite.All                         |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /users/{user-id}/followedSites/remove
```

## <a name="request-body"></a>要求本文

要求本文で、次の表に記載されている id パラメーターを持つ JSON オブジェクトの配列を指定します。 


| 名前                 | 値  | 説明                                                            |
|:---------------------|:-------|:-----------------------------------------------------------------------|
|   id                 | string | アイテムの[一意の識別子](../resources/site.md#id-property)。 |

## <a name="response"></a>応答

* 要求が成功した場合、このメソッドは`204`コンテンツのない状態コードを返します。  
* 指定したサイトのフォローを取り消しているときにエラーが発生した`207`場合、このメソッドは状態コードを返し、応答本文には、[エラーが発生](/graph/errors)していないサイトを示す error オブジェクトと siteids 含むエントリの配列が含まれます。

## <a name="example"></a>例

次の例は、複数のサイトをフォローする方法を示しています。

### <a name="request"></a>要求

<!-- { "blockType": "request", "name": "unfollow-site", "scopes": "sites.readwrite.all" } -->

```http
POST /users/{user-id}/followedSites/remove
Content-Type: application/json

{
    "value":
    [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740"
        },
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851"
        }
    ] 
}
```
### <a name="response"></a>応答

成功した場合、次の JSON 応答を返します。 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 204 No Content
```

エラーが発生した場合は、次の JSON 応答を返します。 

<!-- { "blockType": "response", "@type": "microsoft.graph.site", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 207 Multi-Status
Content-type: application/json

{
    "value": [
        {
            "id": "contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,512a596e-90a1-49e3-9b48-bfa80bee8740",
            "error": {
                "@odata.type": "#oneDrive.error",
                "code": "invalidRequest",
                "message": "The site Id information that is provided in the request is incorrect",
                "innerError": {
                    "code": "invalidRequest",
                    "errorType": "expected",
                    "message": "The site Id information that is provided in the request is incorrect",
                    "stackTrace": "",
                    "throwSite": ""
                }
            }
        }
    ]
}
```  

<!-- {
  "type": "#page.annotation",
  "description": "Unfollow sharepoint site/sites for a user.",
  "keywords": "unfollow site",
  "section": "documentation",
  "tocPath": "Sites/Unfollow site"
} -->
