---
title: SynchronizationSchema を更新します。
description: やテンプレートの特定のジョブ、同期スキーマを更新します。 このメソッドは、要求で提供されるもので、現在のスキーマを完全に置き換えます。 テンプレートのスキーマを更新するには、アプリケーション オブジェクトの呼び出しを確認します。 アプリケーションの所有者でなければなりません。
ms.openlocfilehash: 18ad164f0f1860ce954a9d4e1170f71e47f513b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072010"
---
# <a name="update-synchronizationschema"></a>SynchronizationSchema を更新します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

やテンプレートの特定のジョブ、同期スキーマを更新します。 このメソッドは、要求で提供されるもので、現在のスキーマを完全に置き換えます。 テンプレートのスキーマを更新するには、アプリケーション オブジェクトの呼び出しを確認します。 アプリケーションの所有者でなければなりません。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     |Directory.ReadWrite.All  |
|委任 (個人用 Microsoft アカウント) |サポートされていません。|
|アプリケーション                            |サポートされていません。| 

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PUT /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
PUT /applications/{id}/synchronization/templates/{templateId}/schema
```

## <a name="request-headers"></a>要求ヘッダー

| 名前           | 型    | 説明|
|:---------------|:--------|:-----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

要求の本体では、既存のスキーマを置換する[synchronizationSchema](../resources/synchronization-synchronizationschema.md)オブジェクトを指定します。

## <a name="response"></a>応答

正常終了した場合、`204 No Content`応答コード。 応答本体には何もは返されません。

## <a name="example"></a>例

##### <a name="request"></a>要求
要求の例を次に示します。

>**注:** ここで示すように、要求オブジェクトは、読みやすさの短縮されます。 実際の呼び出しのすべてのプロパティを指定します。
<!-- {
  "blockType": "request",
  "name": "update_synchronizationschema"
}-->
```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema

{
    "directories": [
        {
            "name": "Azure Active Directory",
            "objects": [
                {
                    "name": "User",
                    "attributes": [
                        {
                            "name": "userPrincipalName",
                            "type": "string"
                        }
                    ]
                },
            ]
        },
        {
            "name": "Salesforce",
        }
    ],
    "synchronizationRules":[
        {
            "name": "USER_TO_USER",
            "sourceDirectoryName": "Azure Active Directory",
            "targetDirectoryName": "Salesforce",
            "objectMappings": [
                {
                    "sourceObjectName": "User",
                    "targetObjectName": "User",
                    "attributeMappings": [
                        {
                            "source": {},
                            "targetAttributeName": "userName"
                        },
                    ]
                },
            ]
        },
    ]
}

```

##### <a name="response"></a>応答
応答の例を次に示します。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update synchronizationschema",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->