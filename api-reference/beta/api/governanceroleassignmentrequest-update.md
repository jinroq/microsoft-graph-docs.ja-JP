---
title: GovernanceRoleAssignmentRequests を更新します。
description: 管理者が意思決定を更新するを有効にする (`AdminApproved`または`AdminDenied`) の状態にある governanceRoleAssignmentRequests の`PendingAdminDecision`。
localization_priority: Normal
ms.openlocfilehash: 01178492517ae0ce1e2ed011e749e54af8e5d805
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576529"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="12e30-103">GovernanceRoleAssignmentRequests を更新します。</span><span class="sxs-lookup"><span data-stu-id="12e30-103">Update governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12e30-104">管理者が意思決定を更新するを有効にする (`AdminApproved`または`AdminDenied`) の状態にある[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)の`PendingAdminDecision`。</span><span class="sxs-lookup"><span data-stu-id="12e30-104">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="12e30-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="12e30-105">Permissions</span></span>
<span data-ttu-id="12e30-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12e30-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="12e30-108">**注:** この API では、依頼者の少なくとも 1 つある必要があります`Active`管理者の役割の割り当て (`owner`または`user access administrator`) [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)が属しているリソースにします。</span><span class="sxs-lookup"><span data-stu-id="12e30-108">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="12e30-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12e30-109">Permission type</span></span>      | <span data-ttu-id="12e30-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="12e30-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12e30-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12e30-111">Delegated (work or school account)</span></span> | <span data-ttu-id="12e30-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="12e30-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="12e30-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12e30-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12e30-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12e30-114">Not supported.</span></span>    |
|<span data-ttu-id="12e30-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12e30-115">Application</span></span> | <span data-ttu-id="12e30-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="12e30-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="12e30-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12e30-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="12e30-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12e30-118">Request headers</span></span>
| <span data-ttu-id="12e30-119">名前</span><span class="sxs-lookup"><span data-stu-id="12e30-119">Name</span></span>           | <span data-ttu-id="12e30-120">説明</span><span class="sxs-lookup"><span data-stu-id="12e30-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="12e30-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="12e30-121">Authorization</span></span>  | <span data-ttu-id="12e30-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="12e30-122">Bearer {code}</span></span>|
| <span data-ttu-id="12e30-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="12e30-123">Content-type</span></span>  | <span data-ttu-id="12e30-124">application/json</span><span class="sxs-lookup"><span data-stu-id="12e30-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12e30-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="12e30-125">Request body</span></span>

|<span data-ttu-id="12e30-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="12e30-126">Parameters</span></span>      |<span data-ttu-id="12e30-127">型</span><span class="sxs-lookup"><span data-stu-id="12e30-127">Type</span></span>                   |<span data-ttu-id="12e30-128">必須</span><span class="sxs-lookup"><span data-stu-id="12e30-128">Required</span></span> |<span data-ttu-id="12e30-129">説明</span><span class="sxs-lookup"><span data-stu-id="12e30-129">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="12e30-130">理由</span><span class="sxs-lookup"><span data-stu-id="12e30-130">reason</span></span>        |<span data-ttu-id="12e30-131">String</span><span class="sxs-lookup"><span data-stu-id="12e30-131">String</span></span>                 |<span data-ttu-id="12e30-132">✓</span><span class="sxs-lookup"><span data-stu-id="12e30-132">✓</span></span>        |<span data-ttu-id="12e30-133">彼の意思決定の管理者によって提供されている理由です。</span><span class="sxs-lookup"><span data-stu-id="12e30-133">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="12e30-134">意思決定</span><span class="sxs-lookup"><span data-stu-id="12e30-134">decision</span></span>        |<span data-ttu-id="12e30-135">String</span><span class="sxs-lookup"><span data-stu-id="12e30-135">String</span></span>                 |<span data-ttu-id="12e30-136">✓</span><span class="sxs-lookup"><span data-stu-id="12e30-136">✓</span></span>        |<span data-ttu-id="12e30-137">役割の割り当て要求の管理者の意思決定します。</span><span class="sxs-lookup"><span data-stu-id="12e30-137">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="12e30-138">として値を更新する必要があります`AdminApproved`または`AdminDenied`。</span><span class="sxs-lookup"><span data-stu-id="12e30-138">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="12e30-139">スケジュール</span><span class="sxs-lookup"><span data-stu-id="12e30-139">schedule</span></span>      |[<span data-ttu-id="12e30-140">microsoft.graph.governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="12e30-140"> microsoft.graph.governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="12e30-141">役割の割り当て要求のスケジュールです。</span><span class="sxs-lookup"><span data-stu-id="12e30-141">The schedule of the role assignment request.</span></span> <span data-ttu-id="12e30-142">状態の`AdminApproved`、これは必須です。</span><span class="sxs-lookup"><span data-stu-id="12e30-142">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="12e30-143">assignmentState</span><span class="sxs-lookup"><span data-stu-id="12e30-143">assignmentState</span></span>      |<span data-ttu-id="12e30-144">String</span><span class="sxs-lookup"><span data-stu-id="12e30-144">String</span></span>|         | <span data-ttu-id="12e30-145">割り当て、および値の状態は、`Eligible`または`Active`。</span><span class="sxs-lookup"><span data-stu-id="12e30-145">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="12e30-146">意思決定の`AdminApproved`、これは必須です。</span><span class="sxs-lookup"><span data-stu-id="12e30-146">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="12e30-147">応答</span><span class="sxs-lookup"><span data-stu-id="12e30-147">Response</span></span>
<span data-ttu-id="12e30-148">このメソッドは、要求の状態にあるにのみ適用できます`PendingAdminDecision`。</span><span class="sxs-lookup"><span data-stu-id="12e30-148">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="12e30-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="12e30-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12e30-151">例</span><span class="sxs-lookup"><span data-stu-id="12e30-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="12e30-152">要求</span><span class="sxs-lookup"><span data-stu-id="12e30-152">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
##### <a name="request-body"></a><span data-ttu-id="12e30-153">要求本文</span><span class="sxs-lookup"><span data-stu-id="12e30-153">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="12e30-154">応答</span><span class="sxs-lookup"><span data-stu-id="12e30-154">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UpdateRequest governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
