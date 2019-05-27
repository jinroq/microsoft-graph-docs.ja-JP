---
title: リスト governanceRoleAssignmentRequests
description: 'GovernanceRoleAssignmentRequests のコレクションを取得します。 '
localization_priority: Normal
ms.openlocfilehash: 1f51c2be86424162e1c7003aaed9d34a352cbfa1
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2019
ms.locfileid: "34422452"
---
# <a name="list-governanceroleassignmentrequests"></a><span data-ttu-id="e8753-103">リスト governanceRoleAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="e8753-103">List governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8753-104">[GovernanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e8753-104">Retrieve a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md).</span></span> 

## <a name="permissions"></a><span data-ttu-id="e8753-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e8753-105">Permissions</span></span>
<span data-ttu-id="e8753-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8753-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8753-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e8753-108">Permission type</span></span>      | <span data-ttu-id="e8753-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e8753-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8753-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e8753-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e8753-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="e8753-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="e8753-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e8753-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8753-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8753-113">Not supported.</span></span>    |
|<span data-ttu-id="e8753-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e8753-114">Application</span></span> | <span data-ttu-id="e8753-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8753-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8753-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e8753-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="e8753-117">リソース上の[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e8753-117">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) on a resource.</span></span>
    
><span data-ttu-id="e8753-118">**注:** 要求では、アクセス許可のスコープの他に、リソースに対して少なくとも1つの役割の割り当てが必要になります。</span><span class="sxs-lookup"><span data-stu-id="e8753-118">**Note:** Besides the permission scope, the request requires the requestor to have at least one role assignment on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleAssignmentRequests
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'{resourceId}'
```
<span data-ttu-id="e8753-119">採鉱所の[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e8753-119">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) of mine.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=subjectId+eq+'{myId}'
```

<span data-ttu-id="e8753-120">管理者による決定を保留している[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)のコレクションを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e8753-120">List a collection of [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are pending administrator decisions.</span></span>
    
><span data-ttu-id="e8753-121">**注:** この要求では、アクセス許可スコープに加えて、リソースに対し`Active`て少なくとも`owner` 1 `user access administrator`つの管理者の役割の割り当て (または) をリクエスターが必要とします。</span><span class="sxs-lookup"><span data-stu-id="e8753-121">**Note:** Besides the permission scope, this request requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

```http
GET /privilegedAccess/azureResources/roleAssignmentRequests?$filter=status/subStatus+eq+'PendingAdminDecision'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8753-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e8753-122">Optional query parameters</span></span>
<span data-ttu-id="e8753-123">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e8753-123">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8753-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e8753-124">Request headers</span></span>
| <span data-ttu-id="e8753-125">名前</span><span class="sxs-lookup"><span data-stu-id="e8753-125">Name</span></span>      |<span data-ttu-id="e8753-126">説明</span><span class="sxs-lookup"><span data-stu-id="e8753-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8753-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8753-127">Authorization</span></span>  | <span data-ttu-id="e8753-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="e8753-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8753-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="e8753-129">Request body</span></span>
<span data-ttu-id="e8753-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e8753-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8753-131">応答</span><span class="sxs-lookup"><span data-stu-id="e8753-131">Response</span></span>
<span data-ttu-id="e8753-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e8753-132">If successful, this method returns a `200 OK` response code and a collection of [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8753-133">例</span><span class="sxs-lookup"><span data-stu-id="e8753-133">Example</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroleassignmentrequests"
}-->
<span data-ttu-id="e8753-134">管理者は、サブスクリプション Wingtip Toys-生産に対する保留中の役割の割り当て要求を照会します。</span><span class="sxs-lookup"><span data-stu-id="e8753-134">Administrators query pending role assignment requests for subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="e8753-135">要求</span><span class="sxs-lookup"><span data-stu-id="e8753-135">Request</span></span>

```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests?$filter=resourceId+eq+'e5e7d29d-5465-45ac-885f-4716a5ee74b5'
```
##### <a name="response"></a><span data-ttu-id="e8753-136">応答</span><span class="sxs-lookup"><span data-stu-id="e8753-136">Response</span></span>
<span data-ttu-id="e8753-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e8753-137">Here is an example of the response.</span></span> 

><span data-ttu-id="e8753-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e8753-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
