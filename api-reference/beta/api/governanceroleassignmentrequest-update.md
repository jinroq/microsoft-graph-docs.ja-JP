---
title: GovernanceRoleAssignmentRequests の更新
description: 管理者が、の`AdminApproved` `AdminDenied` `PendingAdminDecision`状態にある governanceRoleAssignmentRequests 上の意思決定 (または) を更新できるようにします。
localization_priority: Normal
ms.openlocfilehash: 03f8d87d75a8edfa9c6b8fdc818114e0b41661ce
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440772"
---
# <a name="update-governanceroleassignmentrequests"></a><span data-ttu-id="8a3c8-103">GovernanceRoleAssignmentRequests の更新</span><span class="sxs-lookup"><span data-stu-id="8a3c8-103">Update governanceRoleAssignmentRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a3c8-104">管理者が`AdminApproved` 、の`AdminDenied` `PendingAdminDecision`状態にある[governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md)上の意思決定 (または) を更新できるようにします。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-104">Enable administrators to update their decisions (`AdminApproved` or `AdminDenied`) on [governanceRoleAssignmentRequests](../resources/governanceroleassignmentrequest.md) that are in status of `PendingAdminDecision`.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a3c8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a3c8-105">Permissions</span></span>
<span data-ttu-id="8a3c8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="8a3c8-108">**注:** この API では、 [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)が属しているリソース`Active`に対して、要求者が少なくとも1つの管理者ロールの割り当て`owner` `user access administrator`を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-108">**Note:** This API also requires that the requester have at least one `Active` adminstrator role assignment (`owner` or `user access administrator`) on the resource that the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) belongs to.</span></span> 

|<span data-ttu-id="8a3c8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8a3c8-109">Permission type</span></span>      | <span data-ttu-id="8a3c8-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8a3c8-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a3c8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8a3c8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8a3c8-112">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="8a3c8-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="8a3c8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8a3c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a3c8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-114">Not supported.</span></span>    |
|<span data-ttu-id="8a3c8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8a3c8-115">Application</span></span> | <span data-ttu-id="8a3c8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8a3c8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8a3c8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/updateRequest   
```

## <a name="request-headers"></a><span data-ttu-id="8a3c8-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8a3c8-118">Request headers</span></span>
| <span data-ttu-id="8a3c8-119">名前</span><span class="sxs-lookup"><span data-stu-id="8a3c8-119">Name</span></span>           | <span data-ttu-id="8a3c8-120">説明</span><span class="sxs-lookup"><span data-stu-id="8a3c8-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8a3c8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a3c8-121">Authorization</span></span>  | <span data-ttu-id="8a3c8-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8a3c8-122">Bearer {code}</span></span>|
| <span data-ttu-id="8a3c8-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="8a3c8-123">Content-type</span></span>  | <span data-ttu-id="8a3c8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8a3c8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a3c8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a3c8-125">Request body</span></span>

|<span data-ttu-id="8a3c8-126">パラメーター</span><span class="sxs-lookup"><span data-stu-id="8a3c8-126">Parameters</span></span>      |<span data-ttu-id="8a3c8-127">型</span><span class="sxs-lookup"><span data-stu-id="8a3c8-127">Type</span></span>                   |<span data-ttu-id="8a3c8-128">必須</span><span class="sxs-lookup"><span data-stu-id="8a3c8-128">Required</span></span> |<span data-ttu-id="8a3c8-129">説明</span><span class="sxs-lookup"><span data-stu-id="8a3c8-129">Description</span></span>|
|:-------------|:----------------------|:--------|:----------|
|<span data-ttu-id="8a3c8-130">したがっ</span><span class="sxs-lookup"><span data-stu-id="8a3c8-130">reason</span></span>        |<span data-ttu-id="8a3c8-131">String</span><span class="sxs-lookup"><span data-stu-id="8a3c8-131">String</span></span>                 |<span data-ttu-id="8a3c8-132">✓</span><span class="sxs-lookup"><span data-stu-id="8a3c8-132">✓</span></span>        |<span data-ttu-id="8a3c8-133">管理者によって決定された理由。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-133">The reason provided by the administrator for his decision.</span></span>|
|<span data-ttu-id="8a3c8-134">条件</span><span class="sxs-lookup"><span data-stu-id="8a3c8-134">decision</span></span>        |<span data-ttu-id="8a3c8-135">String</span><span class="sxs-lookup"><span data-stu-id="8a3c8-135">String</span></span>                 |<span data-ttu-id="8a3c8-136">✓</span><span class="sxs-lookup"><span data-stu-id="8a3c8-136">✓</span></span>        |<span data-ttu-id="8a3c8-137">管理者は、役割の割り当て要求を決定します。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-137">The administrator decision of the role assignment request.</span></span> <span data-ttu-id="8a3c8-138">値をまたは`AdminApproved` `AdminDenied`として更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-138">The value should be updated as `AdminApproved` or `AdminDenied`.</span></span>|
|<span data-ttu-id="8a3c8-139">schedule</span><span class="sxs-lookup"><span data-stu-id="8a3c8-139">schedule</span></span>      |[<span data-ttu-id="8a3c8-140">governanceSchedule</span><span class="sxs-lookup"><span data-stu-id="8a3c8-140">governanceSchedule</span></span>](../resources/governanceschedule.md)|        | <span data-ttu-id="8a3c8-141">役割の割り当て要求のスケジュール。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-141">The schedule of the role assignment request.</span></span> <span data-ttu-id="8a3c8-142">の`AdminApproved`状態については、が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-142">For status of `AdminApproved`, it is required.</span></span>|
|<span data-ttu-id="8a3c8-143">割り当ての状態</span><span class="sxs-lookup"><span data-stu-id="8a3c8-143">assignmentState</span></span>      |<span data-ttu-id="8a3c8-144">String</span><span class="sxs-lookup"><span data-stu-id="8a3c8-144">String</span></span>|         | <span data-ttu-id="8a3c8-145">代入の状態で、値はまたは`Eligible` `Active`で指定できます。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-145">The state of assignment, and the values can be `Eligible` or `Active`.</span></span> <span data-ttu-id="8a3c8-146">について`AdminApproved`は、必須です。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-146">For decision of `AdminApproved`, it is required.</span></span> |
### <a name="response"></a><span data-ttu-id="8a3c8-147">応答</span><span class="sxs-lookup"><span data-stu-id="8a3c8-147">Response</span></span>
<span data-ttu-id="8a3c8-148">このメソッドは、の`PendingAdminDecision`状態にある要求にのみ適用できます。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-148">This method can only be applied to requests that are in status of `PendingAdminDecision`.</span></span>

<span data-ttu-id="8a3c8-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8a3c8-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a3c8-151">例</span><span class="sxs-lookup"><span data-stu-id="8a3c8-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a3c8-152">要求</span><span class="sxs-lookup"><span data-stu-id="8a3c8-152">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8a3c8-153">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8a3c8-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updaterequest_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/updateRequest
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8a3c8-154">C#</span><span class="sxs-lookup"><span data-stu-id="8a3c8-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updaterequest-governanceroleassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8a3c8-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="8a3c8-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updaterequest-governanceroleassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8a3c8-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="8a3c8-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updaterequest-governanceroleassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="request-body"></a><span data-ttu-id="8a3c8-157">要求本文</span><span class="sxs-lookup"><span data-stu-id="8a3c8-157">Request body</span></span>
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

##### <a name="response"></a><span data-ttu-id="8a3c8-158">応答</span><span class="sxs-lookup"><span data-stu-id="8a3c8-158">Response</span></span>
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
  ]
}
-->
