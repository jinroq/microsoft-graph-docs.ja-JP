---
title: GovernanceRoleAssignmentRequest のキャンセル
description: GovernanceRoleAssignmentRequest を取り消します。
localization_priority: Normal
ms.openlocfilehash: 4972c1f283c08b1304c6a01fdc0acc1d6942aec1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593521"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="b79fc-103">GovernanceRoleAssignmentRequest のキャンセル</span><span class="sxs-lookup"><span data-stu-id="b79fc-103">Cancel governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b79fc-104">[GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)を取り消します。</span><span class="sxs-lookup"><span data-stu-id="b79fc-104">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b79fc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b79fc-105">Permissions</span></span>
<span data-ttu-id="b79fc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b79fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b79fc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b79fc-108">Permission type</span></span>      | <span data-ttu-id="b79fc-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b79fc-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b79fc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b79fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b79fc-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="b79fc-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="b79fc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b79fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b79fc-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b79fc-113">Not supported.</span></span>    |
|<span data-ttu-id="b79fc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b79fc-114">Application</span></span> | <span data-ttu-id="b79fc-115">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="b79fc-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="b79fc-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b79fc-116">Optional query parameters</span></span>
<span data-ttu-id="b79fc-117">このメソッドは、 [OData クエリパラメーター](/graph/query-parameters)をサポートし**ていません**。</span><span class="sxs-lookup"><span data-stu-id="b79fc-117">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="b79fc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b79fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="b79fc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b79fc-119">Request headers</span></span>
| <span data-ttu-id="b79fc-120">名前</span><span class="sxs-lookup"><span data-stu-id="b79fc-120">Name</span></span>       | <span data-ttu-id="b79fc-121">説明</span><span class="sxs-lookup"><span data-stu-id="b79fc-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b79fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b79fc-122">Authorization</span></span>  | <span data-ttu-id="b79fc-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b79fc-123">Bearer {code}</span></span>|
| <span data-ttu-id="b79fc-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="b79fc-124">Content-type</span></span>  | <span data-ttu-id="b79fc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b79fc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b79fc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b79fc-126">Request body</span></span>
<span data-ttu-id="b79fc-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b79fc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b79fc-128">応答</span><span class="sxs-lookup"><span data-stu-id="b79fc-128">Response</span></span>
<span data-ttu-id="b79fc-p102">成功した場合、このメソッドは `204 NoContent` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="b79fc-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="b79fc-131">エラー コード</span><span class="sxs-lookup"><span data-stu-id="b79fc-131">Error codes</span></span>
<span data-ttu-id="b79fc-132">この API は、HTTP コードの標準に従います。</span><span class="sxs-lookup"><span data-stu-id="b79fc-132">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="b79fc-133">それに加えて、カスタムエラーコードは以下のとおりです。</span><span class="sxs-lookup"><span data-stu-id="b79fc-133">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="b79fc-134">エラー コード</span><span class="sxs-lookup"><span data-stu-id="b79fc-134">Error code</span></span>     | <span data-ttu-id="b79fc-135">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="b79fc-135">Error message</span></span>              | <span data-ttu-id="b79fc-136">詳細</span><span class="sxs-lookup"><span data-stu-id="b79fc-136">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="b79fc-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="b79fc-137">400 BadRequest</span></span> | <span data-ttu-id="b79fc-138">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="b79fc-138">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="b79fc-139">GovernanceRoleAssignmentRequest は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="b79fc-139">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="b79fc-140">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="b79fc-140">400 BadRequest</span></span> | <span data-ttu-id="b79fc-141">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="b79fc-141">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="b79fc-142">、 `Granted` `PendingApproval`、、の状態の要求のみ`PendingAdminDecision`を取り消すことができます。 `PendingApprovalProvisioning`</span><span class="sxs-lookup"><span data-stu-id="b79fc-142">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="b79fc-143">例</span><span class="sxs-lookup"><span data-stu-id="b79fc-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b79fc-144">要求</span><span class="sxs-lookup"><span data-stu-id="b79fc-144">Request</span></span>
<span data-ttu-id="b79fc-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b79fc-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="b79fc-146">応答</span><span class="sxs-lookup"><span data-stu-id="b79fc-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="b79fc-147">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="b79fc-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b79fc-148">Visual</span><span class="sxs-lookup"><span data-stu-id="b79fc-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/cancel_governanceroleassignmentrequest-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b79fc-149">Java</span><span class="sxs-lookup"><span data-stu-id="b79fc-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/cancel_governanceroleassignmentrequest-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
