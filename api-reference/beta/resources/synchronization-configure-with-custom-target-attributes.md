---
title: カスタムターゲット属性を使用して同期を構成する
description: ターゲットディレクトリで定義されているカスタム属性を含めるように同期スキーマをカスタマイズできます。 この記事では、という`officeCode`新しいフィールドを追加することによって、Salesforce サブスクリプションをカスタマイズする方法について説明します。 Azure Active Directory (Azure AD) から Salesforce への同期をセットアップし、ユーザーごとに、Azure AD の`officeCode` `extensionAttribute10`フィールドの値を使用して、salesforce のフィールドにデータを設定します。
localization_priority: Normal
ms.openlocfilehash: 698c6b1cd05f3146962c9ebd5bd0e52b264a3145
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33621278"
---
# <a name="configure-synchronization-with-custom-target-attributes"></a>カスタムターゲット属性を使用して同期を構成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ターゲットディレクトリで定義されているカスタム属性を含めるように同期スキーマをカスタマイズできます。 この記事では、という`officeCode`新しいフィールドを追加することによって、Salesforce サブスクリプションをカスタマイズする方法について説明します。 Azure Active Directory (Azure AD) から Salesforce への同期をセットアップし、ユーザーごとに、Azure AD の`officeCode` `extensionAttribute10`フィールドの値を使用して、salesforce のフィールドにデータを設定します。

この記事では、 [Azure ポータル](https://portal.azure.com)を使用してテナントへの同期をサポートするアプリケーションが既に追加されていること、アプリケーションの表示名がわかっていること、および Microsoft Graph の認証トークンがあることを前提としています。 認証トークンを取得する方法については、「 [Microsoft Graph を呼び出せるようにアクセストークンを取得](https://developer.microsoft.com/graph/docs/concepts/auth_overview)する」を参照してください。

## <a name="find-the-service-principal-object-by-display-name"></a>表示名でサービスプリンシパルオブジェクトを検索する

次の例は、Salesforce という表示名を持つサービスプリンシパルオブジェクトを検索する方法を示しています。

```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
Authorization: Bearer {Token}

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals(id,appId,displayName)",
    "value": [
    {
        "id": "167e33e9-f80e-490e-b4d8-698d4a80fb3e",
        "appId": "cd3ed3de-93ee-400b-8b19-b61ef44a0f29",
        "displayName": "Salesforce"
    },
    {
        "id": "8cbbb70b-7290-42da-83ee-89fa3517a977",
        "appId": "b0f2e3b1-fe31-4658-b216-44dcaeabb63a",
        "displayName": "salesforce 1"
    },
    {
        "id": "60443998-8cf7-4e61-b05c-a53b658cb5e1",
        "appId": "79079396-c301-405d-900f-e2e0c2439a90",
        "displayName": "Salesforce Sandbox"
    }
    ]
}
```

`{servicePrincipalId}`は`167e33e9-f80e-490e-b4d8-698d4a80fb3e`です。


## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a>サービスプリンシパルのコンテキストで同期ジョブを一覧表示する 

次の例は、 `jobId`で使用する必要があるを取得する方法を示しています。 通常、応答は1つのジョブのみを返します。

```http
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
Authorization: Bearer {Token}

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('60443998-8cf7-4e61-b05c-a53b658cb5e1')/synchronization/jobs",
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {},
            "status": {}
    }
    ]
}
```

`{jobId}`は`SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`です。


## <a name="get-the-synchronization-schema"></a>同期スキーマを取得する
次の例は、同期スキーマを取得する方法を示しています。

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 実際の呼び出しでは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "directories": [
        {
              "id": "66e4a8cc-1b7b-435e-95f8-f06cea133828",
              "name": "Azure Active Directory",
              "objects": [
                {
                    "attributes": [
                        {
                          "anchor": true,
                          "caseExact": false,
                          "defaultValue": null,
                          "metadata": [],
                          "multivalued": false,
                          "mutability": "ReadWrite",
                          "name": "objectId",
                          "required": false,
                          "referencedObjects": [],
                          "type": "String"
                        },
                        {
                          "anchor": false,
                          "caseExact": false,
                          "defaultValue": null,
                          "metadata": [],
                          "multivalued": false,
                          "mutability": "ReadWrite",
                          "name": "streetAddress",
                          "required": false,
                          "referencedObjects": [],
                          "type": "String"
                        }
                    ],
                    "name": "User"
                }
             ]
        },
        {
              "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
              "name": "salesforce.com",
              "objects": []
        }
  ],
 "synchronizationRules": [
        {
          "editable": true,
          "id": "4c5ecfa1-a072-4460-b1c3-4adde3479854",
          "name": "USER_OUTBOUND_USER",
          "objectMappings": [
                {
                    "attributeMappings": [
                            {
                              "defaultValue": "True",
                              "exportMissingReferences": false,
                              "flowBehavior": "FlowWhenChanged",
                              "flowType": "Always",
                              "matchingPriority": 0,
                              "source": {
                                "expression": "Not([IsSoftDeleted])",
                                "name": "Not",
                                "parameters": [
                                  {
                                    "key": "source",
                                    "value": {
                                      "expression": "[IsSoftDeleted]",
                                      "name": "IsSoftDeleted",
                                      "parameters": [],
                                      "type": "Attribute"
                                    }
                                  }
                                ],
                                "type": "Function"
                              },
                              "targetAttributeName": "IsActive"
                            }
                     ],
                    "enabled": true,
                    "flowTypes": "Add, Update, Delete",
                    "name": "Synchronize Azure Active Directory Users to salesforce.com",
                    "scope": null,
                    "sourceObjectName": "User",
                    "targetObjectName": "User"
            }]
        }]
}
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_synchronizationschema-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="add-a-definition-for-the-officecode-attribute-and-a-mapping-between-attributes"></a>Officeecode 属性の定義と属性間のマッピングを追加する

任意のテキストエディター (たとえば、[メモ帳 + +](https://notepad-plus-plus.org/)または[JSON エディタ Online](https://www.jsoneditoronline.org/)) を使用して、次のことを行います。

1. `officeCode`属性の[属性定義](synchronization-attributedefinition.md)を追加します。 

    - [ディレクトリ] で、salesforce.com という名前のディレクトリを見つけ、オブジェクトの配列で、 **User**という名前のディレクトリを見つけます。
    - 次の例に示すように、新しい属性をリストに追加します。名前と種類を指定します。

2. `officeCode`と`extensionAttribute10`の間の[属性マッピング](synchronization-attributemapping.md)を追加します。

    - [[同期ルール](synchronization-synchronizationrule.md)] で、ソースディレクトリとして Azure AD を指定するルールを見つけ、Salesforce.com をターゲット`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`ディレクトリ () として指定します。
    - ルールの[オブジェクトマッピング](synchronization-objectmapping.md)で、ユーザー間のマッピングを検索します`"sourceObjectName": "User",   "targetObjectName": "User"`()。
    - **オブジェクトマッピング**の[attributeMappings](synchronization-attributemapping.md)配列に、次の例に示すように、新しいエントリを追加します。

```json
{  
    "directories": [
    {
        "id": "8ffa6169-f354-4751-9b77-9c00765be92d",
            "name": "salesforce.com",
            "objects": [
            {
                "attributes": [
                        {
                            "name": "officeCode",
                            "type": "String"
                        }
                ],
                "name":"User"
            }]
    }
    ],
    "synchronizationRules": [
        {
        "editable": true,
        "id": "4c5ecfa1-a072-4460-b1c3-4adde3479854",
        "name": "USER_OUTBOUND_USER",
        "objectMappings": [
            {
            "attributeMappings": [
                {
                    "source": {
                            "name": "extensionAttribute10",
                            "type": "Attribute"
                        },
                    "targetAttributeName": "officeCode"
                }
            ],
            "name": "Synchronize Azure Active Directory Users to salesforce.com",
            "scope": null,
            "sourceObjectName": "User",
            "targetObjectName": "User"
            }
        ],
    "priority": 1,
        "sourceDirectoryName": "Azure Active Directory",
        "targetDirectoryName": "salesforce.com"
    }
    ]
}
```

## <a name="save-the-modified-synchronization-schema"></a>変更した同期スキーマを保存する

更新された同期スキーマを保存する場合は、未変更のパーツを含むスキーマ全体を含めるようにしてください。 この要求は、既存のスキーマを、指定したスキーマで置き換えます。

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [..],
    "synchronizationRules": [..]
}

HTTP/1.1 201 No Content
```

スキーマが正常に保存された場合は、同期ジョブの次の反復処理によって、Azure AD 内のすべてのアカウントが再処理され、新しいマッピングがプロビジョニングされたすべてのアカウントに適用されます。
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get the synchronization schema",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-configure-with-custom-target-attributes.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/resources/synchronization-configure-with-custom-target-attributes.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
