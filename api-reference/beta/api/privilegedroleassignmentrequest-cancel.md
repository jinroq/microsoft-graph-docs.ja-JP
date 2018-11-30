---
title: PrivilegedRoleAssignmentRequest をキャンセルします。
description: PrivilegedRoleAssignmentRequest をキャンセルします。
ms.openlocfilehash: 99c1102235e93ca365dcdd0e619bcceac9f396f1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071203"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="35075-103">PrivilegedRoleAssignmentRequest をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="35075-103">Cancel privilegedRoleAssignmentRequest</span></span>

> <span data-ttu-id="35075-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="35075-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35075-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35075-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35075-106">の[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="35075-106">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35075-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="35075-107">Permissions</span></span>
<span data-ttu-id="35075-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35075-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35075-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="35075-110">Permission type</span></span>                        | <span data-ttu-id="35075-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="35075-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="35075-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="35075-112">Delegated (work or school account)</span></span> | <span data-ttu-id="35075-113">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="35075-113">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="35075-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="35075-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35075-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35075-115">Not supported.</span></span> |
|<span data-ttu-id="35075-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="35075-116">Application</span></span>                            | <span data-ttu-id="35075-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35075-117">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="35075-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="35075-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="35075-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35075-119">Request headers</span></span>
| <span data-ttu-id="35075-120">名前</span><span class="sxs-lookup"><span data-stu-id="35075-120">Name</span></span>      |<span data-ttu-id="35075-121">説明</span><span class="sxs-lookup"><span data-stu-id="35075-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="35075-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="35075-122">Authorization</span></span>  | <span data-ttu-id="35075-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="35075-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35075-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="35075-125">Request body</span></span>
<span data-ttu-id="35075-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="35075-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="35075-127">応答</span><span class="sxs-lookup"><span data-stu-id="35075-127">Response</span></span>
<span data-ttu-id="35075-128">成功した場合、このメソッドは `200 Ok` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="35075-128">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="35075-129">[PrivilegedRoleAssignmentRequest] が返されます (../resources/privilegedRoleAssignmentRequest.md)、応答の本文にします。</span><span class="sxs-lookup"><span data-stu-id="35075-129">It returns [privilegedRoleAssignmentRequest] (../resources/privilegedRoleAssignmentRequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="35075-130">エラー コード</span><span class="sxs-lookup"><span data-stu-id="35075-130">Error codes</span></span>
<span data-ttu-id="35075-131">この API では、標準の HTTP エラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="35075-131">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="35075-132">さらに、次の表に記載されているカスタムのエラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="35075-132">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="35075-133">エラー コード</span><span class="sxs-lookup"><span data-stu-id="35075-133">Error code</span></span>     | <span data-ttu-id="35075-134">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="35075-134">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="35075-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="35075-135">400 BadRequest</span></span> | <span data-ttu-id="35075-136">要求 Id は、Null にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="35075-136">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="35075-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="35075-137">400 BadRequest</span></span> | <span data-ttu-id="35075-138">要求 ID が見つからないと要求します。</span><span class="sxs-lookup"><span data-stu-id="35075-138">Request with request ID not found.</span></span> |
| <span data-ttu-id="35075-139">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="35075-139">400 BadRequest</span></span> | <span data-ttu-id="35075-140">キャンセルは、スケジュールおよび PendingApproval の状態でのみ実行できます。</span><span class="sxs-lookup"><span data-stu-id="35075-140">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="35075-141">403 許可されていません。</span><span class="sxs-lookup"><span data-stu-id="35075-141">403 UnAuthorized</span></span> | <span data-ttu-id="35075-142">依頼者がするには [キャンセル] の呼び出し、または見つかりません要求は許可されません。</span><span class="sxs-lookup"><span data-stu-id="35075-142">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="35075-143">例</span><span class="sxs-lookup"><span data-stu-id="35075-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="35075-144">要求</span><span class="sxs-lookup"><span data-stu-id="35075-144">Request</span></span>
<span data-ttu-id="35075-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="35075-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests('7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee')/cancel
```

##### <a name="response"></a><span data-ttu-id="35075-146">応答</span><span class="sxs-lookup"><span data-stu-id="35075-146">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequests"
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
    "userId": "Self"，
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
