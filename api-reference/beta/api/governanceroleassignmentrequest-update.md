---
title: GovernanceRoleAssignmentRequests を更新します。
description: 管理者が意思決定を更新するを有効にする (`AdminApproved`または`AdminDenied`) の状態にある governanceRoleAssignmentRequests の`PendingAdminDecision`。
ms.openlocfilehash: 0f52b810b861e18a679ae8aea4ffdf7fd2d67abd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073958"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="7b109-103">GovernanceRoleAssignmentRequests を更新します。</span><span class="sxs-lookup"><span data-stu-id="7b109-103">Update governanceRoleAssignmentRequests</span></span>

> <span data-ttu-id="7b109-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7b109-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b109-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b109-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b109-106">管理者が意思決定を更新するを有効にする (`AdminApproved`または`AdminDenied`) の状態にある[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)の`PendingAdminDecision`。</span><span class="sxs-lookup"><span data-stu-id="7b109-106">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b109-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7b109-107">Permissions</span></span>
<span data-ttu-id="7b109-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b109-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b109-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7b109-110">Permission type</span></span>      | <span data-ttu-id="7b109-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="7b109-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b109-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b109-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7b109-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="7b109-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="7b109-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b109-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b109-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b109-115">Not supported.</span></span>    |
|<span data-ttu-id="7b109-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b109-116">Application</span></span> | <span data-ttu-id="7b109-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="7b109-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="7b109-118">だけでなく、アクセス許可のスコープは、この API は、リクエスターが 1 つ以上を必要があります`Active`管理者の役割の割り当て (`owner`または`user access administrator`)、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)が属するリソースにします。</span><span class="sxs-lookup"><span data-stu-id="7b109-118">Besides the permission scope, this API requires the requestor to have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource, which the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

## <a name="http-request"></a><span data-ttu-id="7b109-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b109-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

### <a name="request-headers"></a><span data-ttu-id="7b109-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b109-120">Request headers</span></span>
| <span data-ttu-id="7b109-121">名前</span><span class="sxs-lookup"><span data-stu-id="7b109-121">Name</span></span>           | <span data-ttu-id="7b109-122">説明</span><span class="sxs-lookup"><span data-stu-id="7b109-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7b109-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b109-123">Authorization</span></span>  | <span data-ttu-id="7b109-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7b109-124">Bearer {code}</span></span>|
| <span data-ttu-id="7b109-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="7b109-125">Content-type</span></span>  | <span data-ttu-id="7b109-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b109-126">application/json</span></span>|

### <a name="request-body"></a><span data-ttu-id="7b109-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b109-127">Request body</span></span>
|<span data-ttu-id="7b109-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="7b109-128">Parameters</span></span>      |<span data-ttu-id="7b109-129">型</span><span class="sxs-lookup"><span data-stu-id="7b109-129">Type</span></span>                   |<span data-ttu-id="7b109-130">必須</span><span class="sxs-lookup"><span data-stu-id="7b109-130">Required</span></span> |<span data-ttu-id="7b109-131">説明</span><span class="sxs-lookup"><span data-stu-id="7b109-131">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="7b109-132">理由</span><span class="sxs-lookup"><span data-stu-id="7b109-132">reason</span></span>        |<span data-ttu-id="7b109-133">String</span><span class="sxs-lookup"><span data-stu-id="7b109-133">String</span></span>                 |<span data-ttu-id="7b109-134">✓</span><span class="sxs-lookup"><span data-stu-id="7b109-134">✓</span></span>        |<span data-ttu-id="7b109-135">彼の意思決定の管理者によって提供されている理由です。</span><span class="sxs-lookup"><span data-stu-id="7b109-135">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="7b109-136">意思決定</span><span class="sxs-lookup"><span data-stu-id="7b109-136">decision</span></span>        |<span data-ttu-id="7b109-137">String</span><span class="sxs-lookup"><span data-stu-id="7b109-137">String</span></span>                 |<span data-ttu-id="7b109-138">✓</span><span class="sxs-lookup"><span data-stu-id="7b109-138">✓</span></span>        |<span data-ttu-id="7b109-139">役割の割り当て要求の管理者の意思決定します。</span><span class="sxs-lookup"><span data-stu-id="7b109-139">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="7b109-140">として値を更新する必要があります`AdminApproved`または`AdminDenied`。</span><span class="sxs-lookup"><span data-stu-id="7b109-140">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="7b109-141">スケジュール</span><span class="sxs-lookup"><span data-stu-id="7b109-141">schedule</span></span>      |[<span data-ttu-id="7b109-142">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="7b109-142">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="7b109-143">役割の割り当て要求のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="7b109-143">The schedule of the role assignment request.</span></span> <span data-ttu-id="7b109-144">状態の`AdminApproved`、これは必須です。</span><span class="sxs-lookup"><span data-stu-id="7b109-144">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="7b109-145">assignmentState</span><span class="sxs-lookup"><span data-stu-id="7b109-145">assignmentState</span></span>      |<span data-ttu-id="7b109-146">String</span><span class="sxs-lookup"><span data-stu-id="7b109-146">String</span></span>|         | <span data-ttu-id="7b109-147">割り当て、および値の状態は、`Eligible`または`Active`。</span><span class="sxs-lookup"><span data-stu-id="7b109-147">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="7b109-148">意思決定の`AdminApproved`、これは必須です。</span><span class="sxs-lookup"><span data-stu-id="7b109-148">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="7b109-149">応答</span><span class="sxs-lookup"><span data-stu-id="7b109-149">Response</span></span>
<span data-ttu-id="7b109-150">このメソッドは、要求の状態にあるにのみ適用できます`PendingAdminDecision`。</span><span class="sxs-lookup"><span data-stu-id="7b109-150">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="7b109-p106">成功した場合、このメソッドは `204, No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7b109-p106">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="7b109-153">例</span><span class="sxs-lookup"><span data-stu-id="7b109-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b109-154">要求</span><span class="sxs-lookup"><span data-stu-id="7b109-154">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="7b109-155">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b109-155">Request body</span></span>
```json
{
  "reason":"approve the request to extend role assignment",
  "schedule":{
    "type":"Once",
    "startDateTime":"2018-02-20T07:31:13.451Z",
    "stopDateTime":"2018-05-21T07:31:13.451Z",
    },
  "decision":"AdminApproved",
  "assignmentState": "Eligible"
}
```

##### <a name="response"></a><span data-ttu-id="7b109-156">応答</span><span class="sxs-lookup"><span data-stu-id="7b109-156">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->