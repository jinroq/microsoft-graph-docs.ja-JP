---
title: directoryAudits を一覧表示する
description: Microsoft Graph API からの directoryAudit リソース (エンティティ) の list メソッドについて説明します。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5ea475ac8715500e8a2337844b1421728e5573fe
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372665"
---
# <a name="list-directoryaudits"></a>directoryAudits を一覧表示する

Azure Active Directory によって生成された監査ログの一覧を取得します。 これには、Azure AD 内のさまざまなサービスによって生成される監査ログが含まれています。これには、ユーザー、アプリ、デバイスとグループの管理、特権 id 管理 (PIM)、アクセスのレビュー、使用条件、id 保護、パスワード管理 (セルフサービスおよび管理者) などがあります。パスワードのリセット) およびセルフサービスのグループ管理など。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
| :------------------------------------- | :------------------------------------------ |
| 委任 (職場または学校のアカウント)     | 監査ログ。 all および All を参照してください。    |
| 委任 (個人用 Microsoft アカウント) | サポートされていません                               |
| アプリケーション                            | AuditLog.Read.All                           |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /auditLogs/directoryaudits
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするために、次の OData クエリパラメーターをサポートします。 これらのパラメーターを使用する方法の詳細については、[OData クエリ パラメーター](/graph/query_parameters)をご確認ください。

| Name                                                       | 説明                                                                   | 例                                                                     |
| :--------------------------------------------------------- | :---------------------------------------------------------------------------- | :-------------------------------------------------------------------------- |
| [\$仕訳](/graph/query_parameters#filter-parameter)       | 結果 (行) をフィルターします。                                                       | `/auditLogs/directoryAudits?&$filter=createdDateTime le 2018-01-24`         |
| [\$ページのトップへ](/graph/query_parameters#top-parameter)             | 結果のページ サイズを設定します。                                                | `/auditLogs/directoryAudits?$top=1`                                         |
| [\$skiptoken](/graph/query_parameters#skiptoken-parameter) | 複数ページにわたる結果セットから、結果の次のページを取得します。 | `/auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a>Filter パラメーターで\$サポートされている属性

| 属性名                                               | サポートされる演算子 |
| :----------------------------------------------------------- | :------------------ |
| activityDisplayName                                          | eq、startswith      |
| activityDateTime                                             | eq、ge、le          |
| loggedByService                                              | eq                  |
| initiatedBy/user/id                                          | eq                  |
| initiatedBy/user/displayName                                 | eq                  |
| initiatedBy/user/userPrincipalName                           | eq、startswith      |
| initiatedBy/app/appId                                        | eq                  |
| initiatedBy/app/appDisplayName                               | eq                  |
| targetResources/any (t: t/id eq ' {value} ')                    | eq                  |
| targetResources/any (t: t/displayName eq ' {value} ')            | eq                  |
| targetResources/any (x: startswith (x/displayName, ' {value} ')) | startswith          |

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明   |
| :------------ | :------------ |
| Authorization | Bearer {code} |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[directoryaudit](../resources/directoryaudit.md)オブジェクトのコレクションを返します。

## <a name="example"></a>例

### <a name="request"></a>要求

以下は、要求の例です。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit"
}-->

```http
GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryaudit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryaudit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryaudit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryaudit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>応答

以下は、応答の例です。

> **注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryaudit",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 271
```

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditlogs/directoryaudits",
  "value": [{
        "id": "id",
        "category": "UserManagement",
        "correlationId": "da159bfb-54fa-4092-8a38-6e1fa7870e30",
        "result": "success",
        "resultReason": "Successfully added member to group",
        "activityDisplayName": "Add member to group",
        "activityDateTime": "2018-01-09T21:20:02.7215374Z",
        "loggedByService": "Core Directory",
        "initiatedBy": {
            "user": {
                "id": "728309ae-1a37-4937-9afe-e35d964db09b",
                "displayName": "Audry Oliver",
                "userPrincipalName": "bob@wingtiptoysonline.com",
                "ipAddress": "127.0.0.1"
            },
            "app": null
        },
        "targetResources": [{
            "id": "ef7e527d-6c92-4234-8c6d-cf6fdfb57f95",
            "displayName": "Example.com",
            "Type": "Group",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync"}],
            "groupType": "unifiedGroups"
            }],
        }, {
            "id": "1f0e98f5-3161-4c6b-9b50-d488572f2bb7",
            "displayName": null,
            "Type": "User",
            "modifiedProperties": [],
            "userPrincipalName": "bob@contoso.com"
        }],
        "additionalDetails": [{
            "key": "Additional Detail Name",
            "value": "Additional Detail Value"
        }]
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryAudits",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
