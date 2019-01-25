---
title: GovernanceRoleSetting を取得します。
description: プロパティと、governanceRoleSetting の関係を取得します。
localization_priority: Normal
ms.openlocfilehash: 2c432c0f680acd2411d57ab6e4b4a7af21f3350a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511038"
---
# <a name="get-governancerolesetting"></a><span data-ttu-id="6bff6-103">GovernanceRoleSetting を取得します。</span><span class="sxs-lookup"><span data-stu-id="6bff6-103">Get governanceRoleSetting</span></span>


[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6bff6-104">プロパティと、 [governanceRoleSetting](../resources/governancerolesetting.md)の関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="6bff6-104">Retrieve the properties and relationships of a [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6bff6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6bff6-105">Permissions</span></span>
<span data-ttu-id="6bff6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6bff6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6bff6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6bff6-108">Permission type</span></span>      | <span data-ttu-id="6bff6-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6bff6-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6bff6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6bff6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6bff6-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6bff6-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="6bff6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6bff6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6bff6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6bff6-113">Not supported.</span></span>    |
|<span data-ttu-id="6bff6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6bff6-114">Application</span></span> | <span data-ttu-id="6bff6-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="6bff6-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="6bff6-116">以外にも、アクセス許可のスコープは、この API には、 [governanceRoleSetting](../resources/governancerolesetting.md)が属するリソースに 1 つ以上のロールの割り当てを要求元が必要です。</span><span class="sxs-lookup"><span data-stu-id="6bff6-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleSetting](../resources/governancerolesetting.md) belongs to.</span></span>
## <a name="http-request"></a><span data-ttu-id="6bff6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6bff6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6bff6-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6bff6-118">Optional query parameters</span></span>
<span data-ttu-id="6bff6-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6bff6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6bff6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6bff6-120">Request headers</span></span>
| <span data-ttu-id="6bff6-121">名前</span><span class="sxs-lookup"><span data-stu-id="6bff6-121">Name</span></span>      |<span data-ttu-id="6bff6-122">説明</span><span class="sxs-lookup"><span data-stu-id="6bff6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6bff6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bff6-123">Authorization</span></span>  | <span data-ttu-id="6bff6-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6bff6-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bff6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6bff6-125">Request body</span></span>
<span data-ttu-id="6bff6-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6bff6-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6bff6-127">応答</span><span class="sxs-lookup"><span data-stu-id="6bff6-127">Response</span></span>
<span data-ttu-id="6bff6-128">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[governanceRoleSetting](../resources/governancerolesetting.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6bff6-128">If successful, this method returns a `200 OK` response code and a [governanceRoleSetting](../resources/governancerolesetting.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6bff6-129">例</span><span class="sxs-lookup"><span data-stu-id="6bff6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6bff6-130">要求</span><span class="sxs-lookup"><span data-stu-id="6bff6-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governancerolesetting"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/80dc5d6f-8d89-47b3-953f-01dc909ed3f9
```
##### <a name="response"></a><span data-ttu-id="6bff6-131">応答</span><span class="sxs-lookup"><span data-stu-id="6bff6-131">Response</span></span>
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
    "Error: /api-reference/beta/api/governancerolesetting-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
