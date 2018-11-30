---
title: GovernanceRoleAssignmentRequest をキャンセルします。
description: GovernanceRoleAssignmentRequest をキャンセルします。
ms.openlocfilehash: 3e83d47b94f69b124b841f99490a012f2e39a42c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069232"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="3aa92-103">GovernanceRoleAssignmentRequest をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="3aa92-103">Cancel governanceRoleAssignmentRequest</span></span>

> <span data-ttu-id="3aa92-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3aa92-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3aa92-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3aa92-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3aa92-106">の[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="3aa92-106">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3aa92-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3aa92-107">Permissions</span></span>
<span data-ttu-id="3aa92-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3aa92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aa92-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3aa92-110">Permission type</span></span>      | <span data-ttu-id="3aa92-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="3aa92-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3aa92-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3aa92-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3aa92-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3aa92-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="3aa92-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3aa92-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3aa92-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3aa92-115">Not supported.</span></span>    |
|<span data-ttu-id="3aa92-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3aa92-116">Application</span></span> | <span data-ttu-id="3aa92-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="3aa92-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="3aa92-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3aa92-118">Optional query parameters</span></span>
<span data-ttu-id="3aa92-119">このメソッドは [OData クエリ パラメーター](/graph/query-parameters)をサポートして**いません**。</span><span class="sxs-lookup"><span data-stu-id="3aa92-119">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="3aa92-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3aa92-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="3aa92-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3aa92-121">Request headers</span></span>
| <span data-ttu-id="3aa92-122">名前</span><span class="sxs-lookup"><span data-stu-id="3aa92-122">Name</span></span>       | <span data-ttu-id="3aa92-123">説明</span><span class="sxs-lookup"><span data-stu-id="3aa92-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3aa92-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3aa92-124">Authorization</span></span>  | <span data-ttu-id="3aa92-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3aa92-125">Bearer {code}</span></span>|
| <span data-ttu-id="3aa92-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="3aa92-126">Content-type</span></span>  | <span data-ttu-id="3aa92-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3aa92-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3aa92-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3aa92-128">Request body</span></span>
<span data-ttu-id="3aa92-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3aa92-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3aa92-130">応答</span><span class="sxs-lookup"><span data-stu-id="3aa92-130">Response</span></span>
<span data-ttu-id="3aa92-p103">成功した場合、このメソッドは `204 NoContent` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="3aa92-p103">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="3aa92-133">エラー コード</span><span class="sxs-lookup"><span data-stu-id="3aa92-133">Error codes</span></span>
<span data-ttu-id="3aa92-134">この API は、HTTP のコードの標準に準拠します。</span><span class="sxs-lookup"><span data-stu-id="3aa92-134">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="3aa92-135">ほかに、カスタムのエラー コードを以下に示します。</span><span class="sxs-lookup"><span data-stu-id="3aa92-135">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="3aa92-136">エラー コード</span><span class="sxs-lookup"><span data-stu-id="3aa92-136">Error code</span></span>     | <span data-ttu-id="3aa92-137">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="3aa92-137">Error message</span></span>              | <span data-ttu-id="3aa92-138">詳細</span><span class="sxs-lookup"><span data-stu-id="3aa92-138">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="3aa92-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="3aa92-139">400 BadRequest</span></span> | <span data-ttu-id="3aa92-140">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="3aa92-140">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="3aa92-141">GovernanceRoleAssignmentRequest は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="3aa92-141">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="3aa92-142">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="3aa92-142">400 BadRequest</span></span> | <span data-ttu-id="3aa92-143">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="3aa92-143">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="3aa92-144">状態でのみ要求`Granted`、 `PendingApproval`、`PendingApprovalProvisioning`と`PendingAdminDecision`キャンセルすることができます。</span><span class="sxs-lookup"><span data-stu-id="3aa92-144">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="3aa92-145">例</span><span class="sxs-lookup"><span data-stu-id="3aa92-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3aa92-146">要求</span><span class="sxs-lookup"><span data-stu-id="3aa92-146">Request</span></span>
<span data-ttu-id="3aa92-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3aa92-147">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="3aa92-148">応答</span><span class="sxs-lookup"><span data-stu-id="3aa92-148">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->