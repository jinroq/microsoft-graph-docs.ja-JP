---
title: PrivilegedRoleAssignmentRequest のキャンセル
description: PrivilegedRoleAssignmentRequest を取り消します。
localization_priority: Normal
ms.openlocfilehash: dc27edc71956c64d91dcc85e72ddd6c3cd65c793
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34537470"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="d618d-103">PrivilegedRoleAssignmentRequest のキャンセル</span><span class="sxs-lookup"><span data-stu-id="d618d-103">Cancel privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d618d-104">[PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)を取り消します。</span><span class="sxs-lookup"><span data-stu-id="d618d-104">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d618d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d618d-105">Permissions</span></span>
<span data-ttu-id="d618d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d618d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d618d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d618d-108">Permission type</span></span>                        | <span data-ttu-id="d618d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d618d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d618d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d618d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d618d-111">PrivilegedAccess、AzureAD、および Directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="d618d-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d618d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d618d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d618d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d618d-113">Not supported.</span></span> |
|<span data-ttu-id="d618d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d618d-114">Application</span></span>                            | <span data-ttu-id="d618d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d618d-115">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="d618d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d618d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="d618d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d618d-117">Request headers</span></span>
| <span data-ttu-id="d618d-118">名前</span><span class="sxs-lookup"><span data-stu-id="d618d-118">Name</span></span>      |<span data-ttu-id="d618d-119">説明</span><span class="sxs-lookup"><span data-stu-id="d618d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d618d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d618d-120">Authorization</span></span>  | <span data-ttu-id="d618d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d618d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d618d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d618d-123">Request body</span></span>
<span data-ttu-id="d618d-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d618d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d618d-125">応答</span><span class="sxs-lookup"><span data-stu-id="d618d-125">Response</span></span>
<span data-ttu-id="d618d-126">成功した場合、このメソッドは `200 Ok` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d618d-126">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="d618d-127">応答本文で[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="d618d-127">It returns [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="d618d-128">エラー コード</span><span class="sxs-lookup"><span data-stu-id="d618d-128">Error codes</span></span>
<span data-ttu-id="d618d-129">この API は、標準の HTTP エラーコードを返します。</span><span class="sxs-lookup"><span data-stu-id="d618d-129">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="d618d-130">さらに、次の表に示すカスタムエラーコードを返します。</span><span class="sxs-lookup"><span data-stu-id="d618d-130">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="d618d-131">エラー コード</span><span class="sxs-lookup"><span data-stu-id="d618d-131">Error code</span></span>     | <span data-ttu-id="d618d-132">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="d618d-132">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="d618d-133">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d618d-133">400 BadRequest</span></span> | <span data-ttu-id="d618d-134">RequestId を Null にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="d618d-134">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="d618d-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d618d-135">400 BadRequest</span></span> | <span data-ttu-id="d618d-136">要求 ID の要求が見つかりません。</span><span class="sxs-lookup"><span data-stu-id="d618d-136">Request with request ID not found.</span></span> |
| <span data-ttu-id="d618d-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="d618d-137">400 BadRequest</span></span> | <span data-ttu-id="d618d-138">取り消しは、スケジュールされた状態と PendingApproval に対してのみ行うことができます。</span><span class="sxs-lookup"><span data-stu-id="d618d-138">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="d618d-139">403権限がありません</span><span class="sxs-lookup"><span data-stu-id="d618d-139">403 UnAuthorized</span></span> | <span data-ttu-id="d618d-140">要求者が取り消し通話を行うことが許可されていないか、または要求が見つかりません。</span><span class="sxs-lookup"><span data-stu-id="d618d-140">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="d618d-141">例</span><span class="sxs-lookup"><span data-stu-id="d618d-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d618d-142">要求</span><span class="sxs-lookup"><span data-stu-id="d618d-142">Request</span></span>
<span data-ttu-id="d618d-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d618d-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="d618d-144">応答</span><span class="sxs-lookup"><span data-stu-id="d618d-144">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "bcfb11e3-fc0d-49ea-b3d5-7d60a48e5043",
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "Cancelling",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d618d-145">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d618d-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d618d-146">C#</span><span class="sxs-lookup"><span data-stu-id="d618d-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/cancel_privilegedRoleAssignmentRequests-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d618d-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="d618d-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/cancel_privilegedRoleAssignmentRequests-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-cancel.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
