---
title: GovernanceRoleSetting を取得する
description: GovernanceRoleSetting のプロパティとリレーションシップを取得します。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: a12cccc40301cc6648b6f728b40d0550ba45543a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419679"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="c95a8-103">GovernanceRoleSetting を取得する</span><span class="sxs-lookup"><span data-stu-id="c95a8-103">Get governanceRoleSetting</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c95a8-104">[GovernanceRoleSetting](../resources/governancerolesetting.md)のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="c95a8-104">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c95a8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c95a8-105">Permissions</span></span>
<span data-ttu-id="c95a8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c95a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c95a8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c95a8-108">Permission type</span></span>      | <span data-ttu-id="c95a8-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c95a8-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c95a8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c95a8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c95a8-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="c95a8-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="c95a8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c95a8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c95a8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c95a8-113">Not supported.</span></span>    |
|<span data-ttu-id="c95a8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c95a8-114">Application</span></span> | <span data-ttu-id="c95a8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c95a8-115">Not supported.</span></span> |

<span data-ttu-id="c95a8-116">この API は、アクセス許可のスコープに加えて、 [governanceRoleSetting](../resources/governancerolesetting.md)が属しているリソースに対して少なくとも1つの役割の割り当てを要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c95a8-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="c95a8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c95a8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c95a8-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c95a8-118">Optional query parameters</span></span>
<span data-ttu-id="c95a8-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c95a8-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c95a8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c95a8-120">Request headers</span></span>
| <span data-ttu-id="c95a8-121">名前</span><span class="sxs-lookup"><span data-stu-id="c95a8-121">Name</span></span>      |<span data-ttu-id="c95a8-122">説明</span><span class="sxs-lookup"><span data-stu-id="c95a8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c95a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c95a8-123">Authorization</span></span>  | <span data-ttu-id="c95a8-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c95a8-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c95a8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c95a8-125">Request body</span></span>
<span data-ttu-id="c95a8-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c95a8-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c95a8-127">応答</span><span class="sxs-lookup"><span data-stu-id="c95a8-127">Response</span></span>
<span data-ttu-id="c95a8-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[governanceRoleSetting](../resources/governancerolesetting.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c95a8-128">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c95a8-129">例</span><span class="sxs-lookup"><span data-stu-id="c95a8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c95a8-130">要求</span><span class="sxs-lookup"><span data-stu-id="c95a8-130">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c95a8-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c95a8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c95a8-132">C#</span><span class="sxs-lookup"><span data-stu-id="c95a8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c95a8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c95a8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c95a8-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="c95a8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c95a8-135">応答</span><span class="sxs-lookup"><span data-stu-id="c95a8-135">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 370

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleSettings/$entity",
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
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
