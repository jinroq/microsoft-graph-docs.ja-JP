---
title: リスト governanceRoleAssignmentRequests
description: 'GovernanceRoleAssignmentRequests のコレクションを取得します。 '
localization_priority: Normal
ms.openlocfilehash: 5ad26ef352eae93e9c804cfb62f5d00df12e32ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515462"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="836a4-103">リスト governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="836a4-103">List governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="836a4-104">[GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="836a4-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="836a4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="836a4-105">Permissions</span></span>
<span data-ttu-id="836a4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="836a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="836a4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="836a4-108">Permission type</span></span>      | <span data-ttu-id="836a4-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="836a4-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="836a4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="836a4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="836a4-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="836a4-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="836a4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="836a4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="836a4-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="836a4-113">Not supported.</span></span>    |
|<span data-ttu-id="836a4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="836a4-114">Application</span></span> | <span data-ttu-id="836a4-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="836a4-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="836a4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="836a4-116">HTTP request</span></span>
<span data-ttu-id="836a4-117"><!-- { "blockType": "ignored" } -->リソースの[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="836a4-117"><!-- { "blockType": "ignored" } --> List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="836a4-118">**注:** 以外にも、アクセス許可のスコープは、要求には、リソースに 1 つ以上のロールの割り当てを要求元が必要です。</span><span class="sxs-lookup"><span data-stu-id="836a4-118">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="836a4-119">私の[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="836a4-119">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="836a4-120">保留中の管理者の決定事項を[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="836a4-120">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="836a4-121">**注:** この要求だけでなく、アクセス許可のスコープに少なくとも 1 つのリクエスターが必要です`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="836a4-121">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="836a4-122">省略可能なクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="836a4-122">Optional query parameters</span></span>
<span data-ttu-id="836a4-123">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="836a4-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="836a4-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="836a4-124">Request headers</span></span>
| <span data-ttu-id="836a4-125">名前</span><span class="sxs-lookup"><span data-stu-id="836a4-125">Name</span></span>      |<span data-ttu-id="836a4-126">説明</span><span class="sxs-lookup"><span data-stu-id="836a4-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="836a4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="836a4-127">Authorization</span></span>  | <span data-ttu-id="836a4-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="836a4-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="836a4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="836a4-129">Request body</span></span>
<span data-ttu-id="836a4-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="836a4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="836a4-131">応答</span><span class="sxs-lookup"><span data-stu-id="836a4-131">Response</span></span>
<span data-ttu-id="836a4-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="836a4-132">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="836a4-133">例</span><span class="sxs-lookup"><span data-stu-id="836a4-133">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="836a4-134">管理者は、サブスクリプション Wingtip toys 社の商品の保留中の役割の割り当て要求を照会します。</span><span class="sxs-lookup"><span data-stu-id="836a4-134">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="836a4-135">要求</span><span class="sxs-lookup"><span data-stu-id="836a4-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="836a4-136">応答</span><span class="sxs-lookup"><span data-stu-id="836a4-136">Response</span></span>
<span data-ttu-id="836a4-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="836a4-137">Here is an example of the response.</span></span> 

><span data-ttu-id="836a4-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="836a4-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 279

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests",
    "value": [
        {
            "id": "d75c65d8-9e66-44ff-b1cd-1ab0947fde1d",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": "",
            "type": "UserRemove",
            "assignmentState": "Active",
            "requestedDateTime": "2018-01-09T23:41:34.367Z",
            "reason": "Deactivation request",
            "schedule": null,
            "status": {
                "status": "Closed",
                "subStatus": "Revoked",
                "statusDetails": []
            }
        },
        {
            "id": "38f42071-3e81-4191-8c0b-11450fb6b547",
            "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
            "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
            "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
            "linkedEligibleRoleAssignmentId": "",
            "type": "UserAdd",
            "assignmentState": "Active",
            "requestedDateTime": "2018-01-10T20:58:09.163Z",
            "reason": "test activations",
            "status": {
                "status": "Closed",
                "subStatus": "Provisioned",
                "statusDetails": [
                    {
                        "key": "EligibilityRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ExpirationRule",
                        "value": "Grant"
                    },
                    {
                        "key": "MfaRule",
                        "value": "Grant"
                    },
                    {
                        "key": "JustificationRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ActivationDayRule",
                        "value": "Grant"
                    },
                    {
                        "key": "ApprovalRule",
                        "value": "Grant"
                    }
                ]
            },
            "schedule": {
                "type": "Once",
                "startDateTime": "2018-01-10T20:58:11.363914Z",
                "endDateTime": "0001-01-01T00:00:00Z",
                "duration": "PT5H"
            }
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
  "description": "List governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
