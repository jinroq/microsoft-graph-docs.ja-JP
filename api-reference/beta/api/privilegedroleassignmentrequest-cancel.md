---
title: PrivilegedRoleAssignmentRequest のキャンセル
description: PrivilegedRoleAssignmentRequest を取り消します。
localization_priority: Normal
ms.openlocfilehash: 2501d34cc7f3facf635b116369a8235adffa986a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444919"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="af950-103">PrivilegedRoleAssignmentRequest のキャンセル</span><span class="sxs-lookup"><span data-stu-id="af950-103">Cancel privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af950-104">[PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)を取り消します。</span><span class="sxs-lookup"><span data-stu-id="af950-104">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="af950-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="af950-105">Permissions</span></span>
<span data-ttu-id="af950-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af950-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="af950-108">Permission type</span></span>                        | <span data-ttu-id="af950-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="af950-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="af950-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="af950-110">Delegated (work or school account)</span></span> | <span data-ttu-id="af950-111">PrivilegedAccess、AzureAD、および Directory.accessasuser.all。</span><span class="sxs-lookup"><span data-stu-id="af950-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="af950-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="af950-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="af950-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af950-113">Not supported.</span></span> |
|<span data-ttu-id="af950-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="af950-114">Application</span></span>                            | <span data-ttu-id="af950-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af950-115">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="af950-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af950-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="af950-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af950-117">Request headers</span></span>
| <span data-ttu-id="af950-118">名前</span><span class="sxs-lookup"><span data-stu-id="af950-118">Name</span></span>      |<span data-ttu-id="af950-119">説明</span><span class="sxs-lookup"><span data-stu-id="af950-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="af950-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="af950-120">Authorization</span></span>  | <span data-ttu-id="af950-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="af950-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="af950-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="af950-123">Request body</span></span>
<span data-ttu-id="af950-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="af950-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="af950-125">応答</span><span class="sxs-lookup"><span data-stu-id="af950-125">Response</span></span>
<span data-ttu-id="af950-126">成功した場合、このメソッドは `200 Ok` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="af950-126">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="af950-127">応答本文で[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="af950-127">It returns [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="af950-128">エラー コード</span><span class="sxs-lookup"><span data-stu-id="af950-128">Error codes</span></span>
<span data-ttu-id="af950-129">この API は、標準の HTTP エラーコードを返します。</span><span class="sxs-lookup"><span data-stu-id="af950-129">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="af950-130">さらに、次の表に示すカスタムエラーコードを返します。</span><span class="sxs-lookup"><span data-stu-id="af950-130">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="af950-131">エラー コード</span><span class="sxs-lookup"><span data-stu-id="af950-131">Error code</span></span>     | <span data-ttu-id="af950-132">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="af950-132">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="af950-133">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="af950-133">400 BadRequest</span></span> | <span data-ttu-id="af950-134">RequestId を Null にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="af950-134">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="af950-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="af950-135">400 BadRequest</span></span> | <span data-ttu-id="af950-136">要求 ID の要求が見つかりません。</span><span class="sxs-lookup"><span data-stu-id="af950-136">Request with request ID not found.</span></span> |
| <span data-ttu-id="af950-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="af950-137">400 BadRequest</span></span> | <span data-ttu-id="af950-138">取り消しは、スケジュールされた状態と PendingApproval に対してのみ行うことができます。</span><span class="sxs-lookup"><span data-stu-id="af950-138">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="af950-139">403権限がありません</span><span class="sxs-lookup"><span data-stu-id="af950-139">403 UnAuthorized</span></span> | <span data-ttu-id="af950-140">要求者が取り消し通話を行うことが許可されていないか、または要求が見つかりません。</span><span class="sxs-lookup"><span data-stu-id="af950-140">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="af950-141">例</span><span class="sxs-lookup"><span data-stu-id="af950-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="af950-142">要求</span><span class="sxs-lookup"><span data-stu-id="af950-142">Request</span></span>
<span data-ttu-id="af950-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="af950-143">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="af950-144">プロトコル</span><span class="sxs-lookup"><span data-stu-id="af950-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="af950-145">C#</span><span class="sxs-lookup"><span data-stu-id="af950-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cancel-privilegedroleassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="af950-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="af950-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cancel-privilegedroleassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="af950-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="af950-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cancel-privilegedroleassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="af950-148">応答</span><span class="sxs-lookup"><span data-stu-id="af950-148">Response</span></span>
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
  ]
}
-->
