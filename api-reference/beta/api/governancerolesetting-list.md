---
title: リスト governanceRoleSettings
description: リソース上の governanceRoleSettings のコレクションを取得します。
ms.openlocfilehash: 81aa141cecdfce65f8ca2934b2464f5978b96eac
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067271"
---
# <a name="list-governancerolesettings"></a><span data-ttu-id="57bc4-103">リスト governanceRoleSettings</span><span class="sxs-lookup"><span data-stu-id="57bc4-103">List governanceRoleSettings</span></span>

> <span data-ttu-id="57bc4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="57bc4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57bc4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57bc4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="57bc4-106">リソースの[governanceRoleSettings](../resources/governancerolesetting.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="57bc4-106">Retrieve a collection of [governanceRoleSettings](../resources/governancerolesetting.md) on a resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="57bc4-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="57bc4-107">Permissions</span></span>
<span data-ttu-id="57bc4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57bc4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57bc4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="57bc4-110">Permission type</span></span>      | <span data-ttu-id="57bc4-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="57bc4-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57bc4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="57bc4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="57bc4-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="57bc4-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="57bc4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="57bc4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57bc4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57bc4-115">Not supported.</span></span>    |
|<span data-ttu-id="57bc4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="57bc4-116">Application</span></span> | <span data-ttu-id="57bc4-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="57bc4-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="57bc4-118">以外にも、アクセス許可のスコープは、この API にはリソースに 1 つ以上のロールの割り当てを要求元が必要です。</span><span class="sxs-lookup"><span data-stu-id="57bc4-118">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>
## <a name="http-request"></a><span data-ttu-id="57bc4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="57bc4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/<resourceId>/roleSettings
GET /privilegedAccess/azureResources/roleSettings?$filter=resourceId+eq+'<resourceId>'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="57bc4-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="57bc4-120">Optional query parameters</span></span>
<span data-ttu-id="57bc4-121">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="57bc4-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57bc4-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57bc4-122">Request headers</span></span>
| <span data-ttu-id="57bc4-123">名前</span><span class="sxs-lookup"><span data-stu-id="57bc4-123">Name</span></span>      |<span data-ttu-id="57bc4-124">説明</span><span class="sxs-lookup"><span data-stu-id="57bc4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="57bc4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="57bc4-125">Authorization</span></span>  | <span data-ttu-id="57bc4-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="57bc4-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="57bc4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="57bc4-127">Request body</span></span>
<span data-ttu-id="57bc4-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="57bc4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57bc4-129">応答</span><span class="sxs-lookup"><span data-stu-id="57bc4-129">Response</span></span>
<span data-ttu-id="57bc4-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[governanceRoleSetting](../resources/governancerolesetting.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="57bc4-130">If successful, this method returns a `200 OK` response code and collection of [governanceRoleSetting](../resources/governancerolesetting.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57bc4-131">使用例</span><span class="sxs-lookup"><span data-stu-id="57bc4-131">Example</span></span>
<span data-ttu-id="57bc4-132">この例では、管理者が Wingtip Toys の本番環境のリソースの役割の設定を一覧表示方法を示します。</span><span class="sxs-lookup"><span data-stu-id="57bc4-132">This example shows how an administrator lists role settings for the resource Wingtip Toys - Prod.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_governancerolesettings"
}-->
##### <a name="request"></a><span data-ttu-id="57bc4-133">要求</span><span class="sxs-lookup"><span data-stu-id="57bc4-133">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleSettings
```
##### <a name="response"></a><span data-ttu-id="57bc4-134">応答</span><span class="sxs-lookup"><span data-stu-id="57bc4-134">Response</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List governanceRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
