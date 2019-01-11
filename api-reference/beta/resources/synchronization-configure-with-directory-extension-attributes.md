---
title: ディレクトリの拡張属性を使用して同期を構成します。
description: 'Azure Active Directory (AD の Azure) ディレクトリの拡張属性を含むように、同期のスキーマをカスタマイズすることができます。 この資料では、Salesforce の User.CommunityNickname の値を設定するのには、ディレクトリの拡張属性 (**extension_9d98asdfl15980a_Nickname**) を使用する方法について説明します。 このシナリオでは、Azure AD 接続する Azure AD に社内の Windows サーバーの Active Directory からディレクトリの拡張属性の数を提供するように設定があります。 '
localization_priority: Normal
ms.openlocfilehash: 093d78b1e47e412a97ac8a4306c432465e24b5e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850100"
---
# <a name="configure-synchronization-with-directory-extension-attributes"></a><span data-ttu-id="75e2d-105">ディレクトリの拡張属性を使用して同期を構成します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-105">Configure synchronization with directory extension attributes</span></span>

> <span data-ttu-id="75e2d-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="75e2d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="75e2d-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75e2d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="75e2d-108">Azure Active Directory (AD の Azure) ディレクトリの拡張属性を含むように、同期のスキーマをカスタマイズすることができます。</span><span class="sxs-lookup"><span data-stu-id="75e2d-108">You can customize your synchronization schema to include Azure Active Directory (Azure AD) directory extension attributes.</span></span> <span data-ttu-id="75e2d-109">この資料では、Salesforce の User.CommunityNickname の値を設定するのには、ディレクトリの拡張属性 (**extension_9d98asdfl15980a_Nickname**) を使用する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-109">This article describes how to use a directory extension attribute (**extension_9d98asdfl15980a_Nickname**) to populate the value of User.CommunityNickname in Salesforce.</span></span> <span data-ttu-id="75e2d-110">このシナリオでは、Azure AD 接続する Azure AD に社内の Windows サーバーの Active Directory からディレクトリの拡張属性の数を提供するように設定があります。</span><span class="sxs-lookup"><span data-stu-id="75e2d-110">In this scenario, you have Azure AD Connect set up to provision a number of directory extension attributes from Windows Server Active Directory on-premises to Azure AD.</span></span> 

<span data-ttu-id="75e2d-111">この資料では、 [Azure ポータル](https://portal.azure.com)を使ってアプリケーションの表示名がわかっている、テナントの同期をサポートするアプリケーションを既に追加されていると、Graph の認証トークンがあることを想定します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-111">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="75e2d-112">認証トークンを取得する方法の詳細については、 [Microsoft Graph を呼び出すための Get アクセス トークン](https://developer.microsoft.com/graph/docs/concepts/auth_overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75e2d-112">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="75e2d-113">サービスのプリンシパル オブジェクトを表示名で検索します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-113">Find the service principal object by display name</span></span>

<span data-ttu-id="75e2d-114">次の使用例は、表示名が「Salesforce のサンド ボックス」のサービスのプリンシパル オブジェクトを検索する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-114">The following example shows how to find a service principal object with the display name "Salesforce Sandbox".</span></span>

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

<span data-ttu-id="75e2d-115">`{servicePrincipalId}` 、 `60443998-8cf7-4e61-b05c-a53b658cb5e1`。</span><span class="sxs-lookup"><span data-stu-id="75e2d-115">The `{servicePrincipalId}` is `60443998-8cf7-4e61-b05c-a53b658cb5e1`.</span></span>

## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="75e2d-116">サービス ・ プリンシパルのコンテキストの同期ジョブを一覧表示</span><span class="sxs-lookup"><span data-stu-id="75e2d-116">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="75e2d-117">次の使用例は、取得する方法を示します、`jobId`を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="75e2d-117">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="75e2d-118">一般に、応答は、1 つのジョブを返します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-118">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="75e2d-119">`{jobId}` 、 `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`。</span><span class="sxs-lookup"><span data-stu-id="75e2d-119">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>

## <a name="find-the-name-of-the-directory-extension-attribute-you-need"></a><span data-ttu-id="75e2d-120">必要があるディレクトリの拡張属性の名前を検索します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-120">Find the name of the directory extension attribute you need</span></span>

<span data-ttu-id="75e2d-121">拡張属性の完全な名前を必要があります。</span><span class="sxs-lookup"><span data-stu-id="75e2d-121">You'll need the full name of the extension attribute.</span></span> <span data-ttu-id="75e2d-122">( **Extension_9d98asdfl15980a_Nickname**のようになります)、完全な名前がわからない場合は、ディレクトリの拡張属性およびそのコンピューターを調査する方法については、次の情報を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75e2d-122">If you don't know the full name (which should look similar to **extension_9d98asdfl15980a_Nickname**), see the following information about directory extension attributes and how to inspect them:</span></span> 

* [<span data-ttu-id="75e2d-123">カスタム プロパティを持つ Azure AD ディレクトリ スキーマを拡張します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-123">Extending the Azure AD directory schema with custom properties</span></span>](https://azure.microsoft.com/en-us/resources/samples/active-directory-dotnet-graphapi-directoryextensions-web/)
* [<span data-ttu-id="75e2d-124">ディレクトリ スキーマの拡張機能 |グラフ API の概念</span><span class="sxs-lookup"><span data-stu-id="75e2d-124">Directory schema extensions | Graph API concepts</span></span>](https://msdn.microsoft.com/library/azure/ad/graph/howto/azure-ad-graph-api-directory-schema-extensions)


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="75e2d-125">同期スキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="75e2d-125">Get the synchronization schema</span></span>
<span data-ttu-id="75e2d-126">次の例では、同期スキーマを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-126">The following example shows how to get the synchronization schema.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

><span data-ttu-id="75e2d-127">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="75e2d-127">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="75e2d-128">すべてのプロパティは、実際の呼び出しで返されます。</span><span class="sxs-lookup"><span data-stu-id="75e2d-128">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-directory-extension-attribute-and-a-mapping-between-the-attributes"></a><span data-ttu-id="75e2d-129">ディレクトリの拡張機能の属性と属性間のマッピングの定義を追加します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-129">Add a definition for the directory extension attribute, and a mapping between the attributes</span></span>

<span data-ttu-id="75e2d-130">(たとえば、[メモ帳では](https://notepad-plus-plus.org/) [JSON エディター オンライン](https://www.jsoneditoronline.org/)) は、任意のテキスト エディターを使用します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-130">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="75e2d-131">[属性の定義](synchronization-attributedefinition.md)を追加、`extension_9d98asdfl15980a_Nickname`の属性です。</span><span class="sxs-lookup"><span data-stu-id="75e2d-131">Add an [attribute definition](synchronization-attributedefinition.md) for the `extension_9d98asdfl15980a_Nickname` attribute.</span></span> 

    - <span data-ttu-id="75e2d-132">[ディレクトリ] で「Azure Active Directory」という名前ディレクトリを検索し、、オブジェクトの配列の 1 つの名前付き**ユーザー**を検索します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-132">Under directories, find the directory with the name "Azure Active Directory", and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="75e2d-133">次の例に示すように名前と型を指定するボックスの一覧に新しい属性を追加します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-133">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="75e2d-134">Extension_9d98asdfl15980a_Nickname と CommunityNickname の間での[属性のマッピング](synchronization-attributemapping.md)を追加します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-134">Add an [attribute mapping](synchronization-attributemapping.md) between extension_9d98asdfl15980a_Nickname and CommunityNickname.</span></span>

    - <span data-ttu-id="75e2d-135">[SynchronizationRules](synchronization-synchronizationrule.md)、[ソース ディレクトリとターゲット ディレクトリとして Salesforce.com Azure AD を指定するルールを検索します (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`)。</span><span class="sxs-lookup"><span data-stu-id="75e2d-135">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="75e2d-136">ルールの[objectMappings](synchronization-objectmapping.md)のユーザー間のマッピングを検索します (`"sourceObjectName": "User",   "targetObjectName": "User"`)。</span><span class="sxs-lookup"><span data-stu-id="75e2d-136">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="75e2d-137">**ObjectMapping**の[attributeMappings](synchronization-attributemapping.md)配列の例を次に示すように、新しいエントリを追加します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-137">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="75e2d-138">変更された同期スキーマを保存します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-138">Save the modified synchronization schema</span></span>

<span data-ttu-id="75e2d-139">更新された同期スキーマを保存するときは、変更されていない部分を含む、スキーマ全体を含めることを確認します。</span><span class="sxs-lookup"><span data-stu-id="75e2d-139">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="75e2d-140">この要求は、既存のスキーマを提供するものに置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="75e2d-140">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [],
    "synchronizationRules": []
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="75e2d-141">スキーマが正常に保存された場合は、同期ジョブの次回のイテレーションで、Azure の AD 内のすべてのアカウントを再処理を開始し、プロビジョニングされたすべてのアカウントに新しいマッピングが適用されます。</span><span class="sxs-lookup"><span data-stu-id="75e2d-141">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
