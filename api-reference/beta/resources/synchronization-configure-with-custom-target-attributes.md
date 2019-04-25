---
title: カスタムターゲット属性を使用して同期を構成する
description: ターゲットディレクトリで定義されているカスタム属性を含めるように同期スキーマをカスタマイズできます。 この記事では、という`officeCode`新しいフィールドを追加することによって、Salesforce サブスクリプションをカスタマイズする方法について説明します。 azure Active Directory (azure ad) から salesforce への同期をセットアップし、ユーザーごとに、azure AD の`officeCode` `extensionAttribute10`フィールドの値を使用して、salesforce のフィールドにデータを設定します。
localization_priority: Normal
ms.openlocfilehash: 1b0a19bab796f7bd8261ebf898450c07bf1415e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582139"
---
# <a name="configure-synchronization-with-custom-target-attributes"></a><span data-ttu-id="764a8-105">カスタムターゲット属性を使用して同期を構成する</span><span class="sxs-lookup"><span data-stu-id="764a8-105">Configure synchronization with custom target attributes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="764a8-106">ターゲットディレクトリで定義されているカスタム属性を含めるように同期スキーマをカスタマイズできます。</span><span class="sxs-lookup"><span data-stu-id="764a8-106">You can customize your synchronization schema to include custom attributes that are defined in the target directory.</span></span> <span data-ttu-id="764a8-107">この記事では、という`officeCode`新しいフィールドを追加することによって、Salesforce サブスクリプションをカスタマイズする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="764a8-107">This article describes how to customize a Salesforce subscription by adding a new field called `officeCode`.</span></span> <span data-ttu-id="764a8-108">azure Active Directory (azure ad) から salesforce への同期をセットアップし、ユーザーごとに、azure AD の`officeCode` `extensionAttribute10`フィールドの値を使用して、salesforce のフィールドにデータを設定します。</span><span class="sxs-lookup"><span data-stu-id="764a8-108">You set up synchronization from Azure Active Directory (Azure AD) to Salesforce, and for each user, you will populate the `officeCode` field in Salesforce with the value from the `extensionAttribute10` field in Azure AD.</span></span>

<span data-ttu-id="764a8-109">この記事では、 [Azure ポータル](https://portal.azure.com)を使用してテナントへの同期をサポートするアプリケーションが既に追加されていること、アプリケーションの表示名がわかっていること、および Microsoft Graph の認証トークンがあることを前提としています。</span><span class="sxs-lookup"><span data-stu-id="764a8-109">This article assumes that you have already added an application that supports synchronization to your tenant through the [Azure Portal](https://portal.azure.com), that you know the application display name, and that you have an authorization token for Microsoft Graph.</span></span> <span data-ttu-id="764a8-110">認証トークンを取得する方法については、「 [Microsoft Graph を呼び出せるようにアクセストークンを取得](https://developer.microsoft.com/graph/docs/concepts/auth_overview)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="764a8-110">For information about how to get the authorization token, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span>

## <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="764a8-111">表示名でサービスプリンシパルオブジェクトを検索する</span><span class="sxs-lookup"><span data-stu-id="764a8-111">Find the service principal object by display name</span></span>

<span data-ttu-id="764a8-112">次の例は、Salesforce という表示名を持つサービスプリンシパルオブジェクトを検索する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="764a8-112">The following example shows how to find a service principal object with the display name Salesforce.</span></span>

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

<span data-ttu-id="764a8-113">`{servicePrincipalId}`は`167e33e9-f80e-490e-b4d8-698d4a80fb3e`です。</span><span class="sxs-lookup"><span data-stu-id="764a8-113">The `{servicePrincipalId}` is `167e33e9-f80e-490e-b4d8-698d4a80fb3e`.</span></span>


## <a name="list-synchronization-jobs-in-the-context-of-the-service-principal"></a><span data-ttu-id="764a8-114">サービスプリンシパルのコンテキストで同期ジョブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="764a8-114">List synchronization jobs in the context of the service principal</span></span> 

<span data-ttu-id="764a8-115">次の例は、 `jobId`で使用する必要があるを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="764a8-115">The following example shows you how to get the `jobId` that you need to work with.</span></span> <span data-ttu-id="764a8-116">通常、応答は1つのジョブのみを返します。</span><span class="sxs-lookup"><span data-stu-id="764a8-116">Generally, the response returns only one job.</span></span>

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

<span data-ttu-id="764a8-117">`{jobId}`は`SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`です。</span><span class="sxs-lookup"><span data-stu-id="764a8-117">The `{jobId}` is `SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa`.</span></span>


## <a name="get-the-synchronization-schema"></a><span data-ttu-id="764a8-118">同期スキーマを取得する</span><span class="sxs-lookup"><span data-stu-id="764a8-118">Get the synchronization schema</span></span>
<span data-ttu-id="764a8-119">次の例は、同期スキーマを取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="764a8-119">The following example shows how to get the synchronization schema.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_synchronizationschema"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
```

><span data-ttu-id="764a8-120">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="764a8-120">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="764a8-121">実際の呼び出しでは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="764a8-121">All the properties will be returned in an actual call.</span></span>

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

## <a name="add-a-definition-for-the-officecode-attribute-and-a-mapping-between-attributes"></a><span data-ttu-id="764a8-122">officeecode 属性の定義と属性間のマッピングを追加する</span><span class="sxs-lookup"><span data-stu-id="764a8-122">Add a definition for the officeCode attribute and a mapping between attributes</span></span>

<span data-ttu-id="764a8-123">任意のテキストエディター (たとえば、[メモ帳 + +](https://notepad-plus-plus.org/)または[JSON エディタ Online](https://www.jsoneditoronline.org/)) を使用して、次のことを行います。</span><span class="sxs-lookup"><span data-stu-id="764a8-123">Use a plain text editor of your choice (for example, [Notepad++](https://notepad-plus-plus.org/) or [JSON Editor Online](https://www.jsoneditoronline.org/)) to:</span></span>

1. <span data-ttu-id="764a8-124">`officeCode`属性の[属性定義](synchronization-attributedefinition.md)を追加します。</span><span class="sxs-lookup"><span data-stu-id="764a8-124">Add an [attribute definition](synchronization-attributedefinition.md) for the `officeCode` attribute.</span></span> 

    - <span data-ttu-id="764a8-125">[ディレクトリ] で、salesforce.com という名前のディレクトリを見つけ、オブジェクトの配列で、 **User**という名前のディレクトリを見つけます。</span><span class="sxs-lookup"><span data-stu-id="764a8-125">Under directories, find the directory with the name salesforce.com, and in the object's array, find the one named **User**.</span></span>
    - <span data-ttu-id="764a8-126">次の例に示すように、新しい属性をリストに追加します。名前と種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="764a8-126">Add the new attribute to the list, specifying the name and type, as shown in the following example.</span></span>

2. <span data-ttu-id="764a8-127">`officeCode`と`extensionAttribute10`の間の[属性マッピング](synchronization-attributemapping.md)を追加します。</span><span class="sxs-lookup"><span data-stu-id="764a8-127">Add an [attribute mapping](synchronization-attributemapping.md) between `officeCode` and `extensionAttribute10`.</span></span>

    - <span data-ttu-id="764a8-128">[[同期ルール](synchronization-synchronizationrule.md)] で、ソースディレクトリとして Azure AD を指定するルールを見つけ、Salesforce.com をターゲット`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`ディレクトリ () として指定します。</span><span class="sxs-lookup"><span data-stu-id="764a8-128">Under [synchronizationRules](synchronization-synchronizationrule.md), find the rule that specifies Azure AD as the source directory, and Salesforce.com as the target directory (`"sourceDirectoryName": "Azure Active Directory",   "targetDirectoryName": "salesforce.com"`).</span></span>
    - <span data-ttu-id="764a8-129">ルールの[オブジェクトマッピング](synchronization-objectmapping.md)で、ユーザー間のマッピングを検索します`"sourceObjectName": "User",   "targetObjectName": "User"`()。</span><span class="sxs-lookup"><span data-stu-id="764a8-129">In the [objectMappings](synchronization-objectmapping.md) of the rule, find the mapping between users (`"sourceObjectName": "User",   "targetObjectName": "User"`).</span></span>
    - <span data-ttu-id="764a8-130">**オブジェクトマッピング**の[attributeMappings](synchronization-attributemapping.md)配列に、次の例に示すように、新しいエントリを追加します。</span><span class="sxs-lookup"><span data-stu-id="764a8-130">In the [attributeMappings](synchronization-attributemapping.md) array of the **objectMapping**, add a new entry, as shown in the following example.</span></span>

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

## <a name="save-the-modified-synchronization-schema"></a><span data-ttu-id="764a8-131">変更した同期スキーマを保存する</span><span class="sxs-lookup"><span data-stu-id="764a8-131">Save the modified synchronization schema</span></span>

<span data-ttu-id="764a8-132">更新された同期スキーマを保存する場合は、未変更のパーツを含むスキーマ全体を含めるようにしてください。</span><span class="sxs-lookup"><span data-stu-id="764a8-132">When you save the updated synchronization schema, make sure that you include the entire schema, including the unmodified parts.</span></span> <span data-ttu-id="764a8-133">この要求は、既存のスキーマを、指定したスキーマで置き換えます。</span><span class="sxs-lookup"><span data-stu-id="764a8-133">This request will replace the existing schema with the one that you provide.</span></span>

```http
PUT https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema
Authorization: Bearer {Token}
{
    "directories": [..],
    "synchronizationRules": [..]
}

HTTP/1.1 201 No Content
```

<span data-ttu-id="764a8-134">スキーマが正常に保存された場合は、同期ジョブの次の反復処理によって、Azure AD 内のすべてのアカウントが再処理され、新しいマッピングがプロビジョニングされたすべてのアカウントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="764a8-134">If the schema was saved successfully, on the next iteration of the synchronization job, it will start re-processing all the accounts in your Azure AD, and the new mappings will be applied to all provisioned accounts.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-configure-with-custom-target-attributes.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
