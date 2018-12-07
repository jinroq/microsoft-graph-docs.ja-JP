---
title: リスト governanceRoleAssignmentRequests
description: 'GovernanceRoleAssignmentRequests のコレクションを取得します。 '
ms.openlocfilehash: 89cb6130b586a44723ec636cbdbe311e0bf8d510
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191159"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="4a161-103">リスト governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="4a161-103">List governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="4a161-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a161-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a161-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a161-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a161-106">[GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4a161-106">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="4a161-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4a161-107">Permissions</span></span>
<span data-ttu-id="4a161-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a161-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a161-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a161-110">Permission type</span></span>      | <span data-ttu-id="4a161-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="4a161-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a161-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a161-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4a161-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="4a161-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="4a161-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a161-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a161-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a161-115">Not supported.</span></span>    |
|<span data-ttu-id="4a161-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a161-116">Application</span></span> | <span data-ttu-id="4a161-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="4a161-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a161-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a161-118">HTTP request</span></span>
<span data-ttu-id="4a161-119"><!-- { "blockType": "ignored" } -->リソースの[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="4a161-119"><!-- { "blockType": "ignored" } --> List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="4a161-120">**注:** 以外にも、アクセス許可のスコープは、要求には、リソースに 1 つ以上のロールの割り当てを要求元が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a161-120">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="4a161-121">私の[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="4a161-121">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="4a161-122">保留中の管理者の決定事項を[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)の一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="4a161-122">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="4a161-123">**注:** この要求だけでなく、アクセス許可のスコープに少なくとも 1 つのリクエスターが必要です`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、リソースにします。</span><span class="sxs-lookup"><span data-stu-id="4a161-123">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a161-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4a161-124">Optional query parameters</span></span>
<span data-ttu-id="4a161-125">このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4a161-125">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a161-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a161-126">Request headers</span></span>
| <span data-ttu-id="4a161-127">名前</span><span class="sxs-lookup"><span data-stu-id="4a161-127">Name</span></span>      |<span data-ttu-id="4a161-128">説明</span><span class="sxs-lookup"><span data-stu-id="4a161-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4a161-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a161-129">Authorization</span></span>  | <span data-ttu-id="4a161-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4a161-130">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a161-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a161-131">Request body</span></span>
<span data-ttu-id="4a161-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4a161-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a161-133">応答</span><span class="sxs-lookup"><span data-stu-id="4a161-133">Response</span></span>
<span data-ttu-id="4a161-134">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4a161-134">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a161-135">例</span><span class="sxs-lookup"><span data-stu-id="4a161-135">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="4a161-136">管理者は、サブスクリプション Wingtip toys 社の商品の保留中の役割の割り当て要求を照会します。</span><span class="sxs-lookup"><span data-stu-id="4a161-136">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="4a161-137">要求</span><span class="sxs-lookup"><span data-stu-id="4a161-137">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="4a161-138">応答</span><span class="sxs-lookup"><span data-stu-id="4a161-138">Response</span></span>
<span data-ttu-id="4a161-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4a161-139">Here is an example of the response.</span></span> 

><span data-ttu-id="4a161-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4a161-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List governanceRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
