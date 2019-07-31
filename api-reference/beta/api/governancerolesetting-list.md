---
title: リスト governanceRoleSettings
description: リソース上の governanceRoleSettings のコレクションを取得します。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 4c9b58480f0b1033a997721b257054be1519ac27
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954103"
---
# <a name="list-governancerolesettings"></a><span data-ttu-id="f6fe9-103">リスト governanceRoleSettings</span><span class="sxs-lookup"><span data-stu-id="f6fe9-103">List governanceRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6fe9-104">リソース上の[governanceRoleSettings](../resources/governancerolesetting.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f6fe9-104">Retrieve a collection of [governanceRoleSettings](../resources/governancerolesetting.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6fe9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f6fe9-105">Permissions</span></span>
<span data-ttu-id="f6fe9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6fe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6fe9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6fe9-108">Permission type</span></span>      | <span data-ttu-id="f6fe9-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f6fe9-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6fe9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f6fe9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f6fe9-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="f6fe9-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f6fe9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6fe9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6fe9-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6fe9-113">Not supported.</span></span>    |
|<span data-ttu-id="f6fe9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6fe9-114">Application</span></span> | <span data-ttu-id="f6fe9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6fe9-115">Not supported.</span></span> |

<span data-ttu-id="f6fe9-116">この API は、アクセス許可スコープの他に、リソースに対して少なくとも1つの役割の割り当てを要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f6fe9-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>
## <a name="http-request"></a><span data-ttu-id="f6fe9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6fe9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/<resourceId>/roleSettings
GET /privilegedAccess/azureResources/roleSettings?$filter=resourceId+eq+'<resourceId>'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f6fe9-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f6fe9-118">Optional query parameters</span></span>
<span data-ttu-id="f6fe9-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f6fe9-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6fe9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6fe9-120">Request headers</span></span>
| <span data-ttu-id="f6fe9-121">名前</span><span class="sxs-lookup"><span data-stu-id="f6fe9-121">Name</span></span>      |<span data-ttu-id="f6fe9-122">説明</span><span class="sxs-lookup"><span data-stu-id="f6fe9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f6fe9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6fe9-123">Authorization</span></span>  | <span data-ttu-id="f6fe9-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f6fe9-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6fe9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6fe9-125">Request body</span></span>
<span data-ttu-id="f6fe9-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f6fe9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6fe9-127">応答</span><span class="sxs-lookup"><span data-stu-id="f6fe9-127">Response</span></span>
<span data-ttu-id="f6fe9-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[governanceRoleSetting](../resources/governancerolesetting.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f6fe9-128">If successful, this method returns a `200 OK` response code and collection of [governanceRoleSetting](../resources/governancerolesetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6fe9-129">例</span><span class="sxs-lookup"><span data-stu-id="f6fe9-129">Example</span></span>
<span data-ttu-id="f6fe9-130">この例では、管理者が、Wingtip Toys のリソースの役割設定を一覧表示する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="f6fe9-130">This example shows how an administrator lists role settings for the resource Wingtip Toys - Prod.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_governancerolesettings"
}-->
##### <a name="request"></a><span data-ttu-id="f6fe9-131">要求</span><span class="sxs-lookup"><span data-stu-id="f6fe9-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleSettings
```
##### <a name="response"></a><span data-ttu-id="f6fe9-132">応答</span><span class="sxs-lookup"><span data-stu-id="f6fe9-132">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 463

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleSettings",
    "value": [
        {
            "id": "80dc5d6f-8d89-47b3-953f-01dc909ed3f9",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "5b8bea96-e9f6-4c63-a8e9-fb092c79f0a1",
            "isDefault": false,
            "lastUpdatedDateTime": "2018-03-26T21:21:43.113Z",
            "lastUpdatedBy": "Vishal Seri",
            "adminEligibleSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
                }
            ],
            "adminMemberSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":43200}"
                },
                {
                    "ruleIdentifier": "MfaRule",
                    "setting": "{\"mfaRequired\":false}"
                },
                {
                    "ruleIdentifier": "JustificationRule",
                    "setting": "{\"required\":true}"
                }
            ],
            "userEligibleSettings": [],
            "userMemberSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":480}"
                },
                {
                    "ruleIdentifier": "MfaRule",
                    "setting": "{\"mfaRequired\":false}"
                },
                {
                    "ruleIdentifier": "JustificationRule",
                    "setting": "{\"required\":true}"
                },
                {
                    "ruleIdentifier": "ApprovalRule",
                    "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"20083cf1-b8d8-43be-9d37-96adfb09e619\",\"Type\":\"User\",\"DisplayName\":\"Vishal Seri\",\"Email\":\"viseri@fimdev.net\"},{\"Id\":\"d158e1b0-5080-4088-a1e7-9ca54f39eb53\",\"Type\":\"User\",\"DisplayName\":\"viseri\",\"Email\":\"viseri@microsoft.com\"}],\"BusinessFlowId\":\"8df9e93a-6ba9-4453-af43-07cb95435032\"}"
                }
            ]
        },
        {
            "id": "ac642250-9c22-4ec5-a072-02e06c1ef3a0",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "688de08e-66d4-4efe-b234-1cf476a603b9",
            "isDefault": false,
            "lastUpdatedDateTime": "2017-12-07T18:12:43.417Z",
            "lastUpdatedBy": "Debashis Choudhury",
            "adminEligibleSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
                }
            ],
            "adminMemberSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":43200}"
                },
                {
                    "ruleIdentifier": "MfaRule",
                    "setting": "{\"mfaRequired\":false}"
                },
                {
                    "ruleIdentifier": "JustificationRule",
                    "setting": "{\"required\":true}"
                }
            ],
            "userEligibleSettings": [],
            "userMemberSettings": [
                {
                    "ruleIdentifier": "ExpirationRule",
                    "setting": "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":480}"
                },
                {
                    "ruleIdentifier": "MfaRule",
                    "setting": "{\"mfaRequired\":false}"
                },
                {
                    "ruleIdentifier": "JustificationRule",
                    "setting": "{\"required\":true}"
                },
                {
                    "ruleIdentifier": "ApprovalRule",
                    "setting": "{\"Enabled\":true,\"Approvers\":[{\"Id\":\"c178dfee-7236-44b5-a363-e15fc63d91f0\",\"Type\":\"User\",\"DisplayName\":\"Debashis Choudhury\",\"Email\":\"debac@fimdev.net\"}],\"BusinessFlowId\":\"fa7d0b98-ed15-47cd-b3e2-aa6bd3e6533a\"}"
                }
            ]
        },
        ...
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List governanceRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
