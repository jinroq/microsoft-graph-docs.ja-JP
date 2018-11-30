---
title: ディレクトリの拡張属性を使用して同期を構成します。
description: 'Azure Active Directory (AD の Azure) ディレクトリの拡張属性を含むように、同期のスキーマをカスタマイズすることができます。 この資料では、Salesforce の User.CommunityNickname の値を設定するのには、ディレクトリの拡張属性 (**extension_9d98asdfl15980a_Nickname**) を使用する方法について説明します。 このシナリオでは、Azure AD 接続する Azure AD に社内の Windows サーバーの Active Directory からディレクトリの拡張属性の数を提供するように設定があります。 '
ms.openlocfilehash: fa29e405b235107cd6773444085e7b409441c90e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073120"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a>ディレクトリの拡張属性を使用して同期を構成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure Active Directory (AD の Azure) ディレクトリの拡張属性を含むように、同期のスキーマをカスタマイズすることができます。 この資料では、Salesforce の User.CommunityNickname の値を設定するのには、ディレクトリの拡張属性 (**extension_9d98asdfl15980a_Nickname**) を使用する方法について説明します。 このシナリオでは、Azure AD 接続する Azure AD に社内の Windows サーバーの Active Directory からディレクトリの拡張属性の数を提供するように設定があります。 

この資料では、 [Azure ポータル](https://portal.azure.com)を使ってアプリケーションの表示名がわかっている、テナントの同期をサポートするアプリケーションを既に追加されていると、Graph の認証トークンがあることを想定します。 認証トークンを取得する方法の詳細については、 [Microsoft Graph を呼び出すための Get アクセス トークン](https://developer.microsoft.com/graph/docs/concepts/auth_overview)を参照してください。

## <a name="find-the-service-principal-object-by-display-name"></a>サービスのプリンシパル オブジェクトを表示名で検索します。

次の使用例は、表示名が「Salesforce のサンド ボックス」のサービスのプリンシパル オブジェクトを検索する方法を示します。

```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
Authorization: Bearer {Token}
```

```json
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

`{servicePrincipalId}` 、 `60443998-8cf7-4e61-b05c-a53b658cb5e1`。

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a>サービス ・ プリンシパルのコンテキストの同期ジョブを一覧表示 

次の使用例は、取得する方法を示します、`jobId`を使用する必要があります。 一般に、応答は、1 つのジョブを返します。

```http
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
Authorization: Bearer {Token}
```

```json
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

`{jobId}` 、 `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`。

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a>必要があるディレクトリの拡張属性の名前を検索します。

拡張属性の完全な名前を必要があります。 ( **Extension_9d98asdfl15980a_Nickname**のようになります)、完全な名前がわからない場合は、ディレクトリの拡張属性およびそのコンピューターを調査する方法については、次の情報を参照してください。 

* [カスタム プロパティを持つ Azure AD ディレクトリ スキーマを拡張します。](https://azure.microsoft.com/en-us/resources/samples/active-directory-dotnet-graphapi-directoryextensions-web/)
* [ディレクトリ スキーマの拡張機能 |グラフ API の概念](https://msdn.microsoft.com/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a>同期スキーマを取得します
次の例では、同期スキーマを取得する方法を示します。

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

>**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。 すべてのプロパティは、実際の呼び出しで返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationSchema"
} -->
```http
HTTP/1.1 200 OK

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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a>ディレクトリの拡張機能の属性と属性間のマッピングの定義を追加します。

(たとえば、[メモ帳では](https://notepad-plus-plus.org/) [JSON エディター オンライン](https://www.jsoneditoronline.org/)) は、任意のテキスト エディターを使用します。

1. [属性の定義](synchronization-attributedefinition.md)を追加、`extension_9d98asdfl15980a_Nickname`の属性です。 

    - [ディレクトリ] で「Azure Active Directory」という名前ディレクトリを検索し、、オブジェクトの配列の 1 つの名前付き**ユーザー**を検索します。
    - 次の例に示すように名前と型を指定するボックスの一覧に新しい属性を追加します。

2. Extension_9d98asdfl15980a_Nickname と CommunityNickname の間での[属性のマッピング](synchronization-attributemapping.md)を追加します。

    - [SynchronizationRules](synchronization-synchronizationrule.md)、[ソース ディレクトリとターゲット ディレクトリとして Salesforce.com Azure AD を指定するルールを検索します (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`)。
    - ルールの[objectMappings](synchronization-objectmapping.md)のユーザー間のマッピングを検索します (`"sourceObjectName": "User",   "targetObjectName": "User"`)。
    - **ObjectMapping**の[attributeMappings](synchronization-attributemapping.md)配列の例を次に示すように、新しいエントリを追加します。

    ```json
    {
        "directories": [
            {
                "id": "66e4a8cc-1b7b-435e-95f8-f06cea133828",
                "name": "Azure Active Directory",
                "objects": [
                    {
                        "attributes": [
                                ,{
                                "name": "extension_9d98asdfl15980a_Nickname",
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
            "metadata": [..],
            "name": "USER_OUTBOUND_USER",
            "objectMappings": [
                {
                    "attributeMappings": [
                    ,{
                        "source": {
                            "name": "extension_9d98asdfl15980a_Nickname",
                            "type": "Attribute"
                        },
                        "targetAttributeName": "CommunityNickname"
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
            },
        ]
    }
    ```

## <a name="save-the-modified-synchronization-schema"></a>変更された同期スキーマを保存します。

更新された同期スキーマを保存するときは、変更されていない部分を含む、スキーマ全体を含めることを確認します。 この要求は、既存のスキーマを提供するものに置き換えられます。

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

スキーマが正常に保存された場合は、同期ジョブの次回のイテレーションで、Azure の AD 内のすべてのアカウントを再処理を開始し、プロビジョニングされたすべてのアカウントに新しいマッピングが適用されます。