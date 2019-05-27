---
title: GovernanceRoleSetting を取得する
description: GovernanceRoleSetting のプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 988fc237e76c0ec653fff768a617a08d33a6998e
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422347"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="a9a4e-103">GovernanceRoleSetting を取得する</span><span class="sxs-lookup"><span data-stu-id="a9a4e-103">Get governanceRoleSetting</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9a4e-104">[GovernanceRoleSetting](../resources/governancerolesetting.md)のプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-104">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a9a4e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a9a4e-105">Permissions</span></span>
<span data-ttu-id="a9a4e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9a4e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9a4e-108">Permission type</span></span>      | <span data-ttu-id="a9a4e-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a9a4e-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9a4e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9a4e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a9a4e-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="a9a4e-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="a9a4e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9a4e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9a4e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-113">Not supported.</span></span>    |
|<span data-ttu-id="a9a4e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9a4e-114">Application</span></span> | <span data-ttu-id="a9a4e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-115">Not supported.</span></span> |

<span data-ttu-id="a9a4e-116">この API は、アクセス許可のスコープに加えて、 [governanceRoleSetting](../resources/governancerolesetting.md)が属しているリソースに対して少なくとも1つの役割の割り当てを要求する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="a9a4e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9a4e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a9a4e-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a9a4e-118">Optional query parameters</span></span>
<span data-ttu-id="a9a4e-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9a4e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9a4e-120">Request headers</span></span>
| <span data-ttu-id="a9a4e-121">名前</span><span class="sxs-lookup"><span data-stu-id="a9a4e-121">Name</span></span>      |<span data-ttu-id="a9a4e-122">説明</span><span class="sxs-lookup"><span data-stu-id="a9a4e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a9a4e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9a4e-123">Authorization</span></span>  | <span data-ttu-id="a9a4e-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a9a4e-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9a4e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9a4e-125">Request body</span></span>
<span data-ttu-id="a9a4e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a9a4e-127">応答</span><span class="sxs-lookup"><span data-stu-id="a9a4e-127">Response</span></span>
<span data-ttu-id="a9a4e-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[governanceRoleSetting](../resources/governancerolesetting.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-128">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a9a4e-129">例</span><span class="sxs-lookup"><span data-stu-id="a9a4e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a9a4e-130">要求</span><span class="sxs-lookup"><span data-stu-id="a9a4e-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
##### <a name="response"></a><span data-ttu-id="a9a4e-131">応答</span><span class="sxs-lookup"><span data-stu-id="a9a4e-131">Response</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a9a4e-132">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="a9a4e-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a9a4e-133">C#</span><span class="sxs-lookup"><span data-stu-id="a9a4e-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_governancerolesetting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9a4e-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="a9a4e-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_governancerolesetting-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/governancerolesetting-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governancerolesetting-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
