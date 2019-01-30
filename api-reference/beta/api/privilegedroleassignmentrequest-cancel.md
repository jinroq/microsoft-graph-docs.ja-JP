---
title: PrivilegedRoleAssignmentRequest をキャンセルします。
description: PrivilegedRoleAssignmentRequest をキャンセルします。
localization_priority: Normal
ms.openlocfilehash: 0cca3f33e6e027c18e24862dc4736006058f8e41
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642808"
---
# <a name="cancel-privilegedroleassignmentrequest"></a><span data-ttu-id="c5491-103">PrivilegedRoleAssignmentRequest をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="c5491-103">Cancel privilegedRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5491-104">の[privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md)をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="c5491-104">Cancel a [privilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c5491-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c5491-105">Permissions</span></span>
<span data-ttu-id="c5491-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5491-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c5491-108">Permission type</span></span>                        | <span data-ttu-id="c5491-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c5491-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5491-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c5491-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c5491-111">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5491-111">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c5491-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c5491-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5491-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5491-113">Not supported.</span></span> |
|<span data-ttu-id="c5491-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c5491-114">Application</span></span>                            | <span data-ttu-id="c5491-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5491-115">Not supported.</span></span> |


### <a name="http-request"></a><span data-ttu-id="c5491-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c5491-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests({requestid})/cancel
```

## <a name="request-headers"></a><span data-ttu-id="c5491-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5491-117">Request headers</span></span>
| <span data-ttu-id="c5491-118">名前</span><span class="sxs-lookup"><span data-stu-id="c5491-118">Name</span></span>      |<span data-ttu-id="c5491-119">説明</span><span class="sxs-lookup"><span data-stu-id="c5491-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c5491-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5491-120">Authorization</span></span>  | <span data-ttu-id="c5491-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c5491-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5491-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="c5491-123">Request body</span></span>
<span data-ttu-id="c5491-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c5491-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5491-125">応答</span><span class="sxs-lookup"><span data-stu-id="c5491-125">Response</span></span>
<span data-ttu-id="c5491-126">成功した場合、このメソッドは `200 Ok` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c5491-126">If successful, this method returns a `200 Ok` response code.</span></span> <span data-ttu-id="c5491-127">[PrivilegedRoleAssignmentRequest] が返されます (../resources/privilegedRoleAssignmentRequest.md)、応答の本文にします。</span><span class="sxs-lookup"><span data-stu-id="c5491-127">It returns [privilegedRoleAssignmentRequest] (../resources/privilegedRoleAssignmentRequest.md) in the response body.</span></span>

### <a name="error-codes"></a><span data-ttu-id="c5491-128">エラー コード</span><span class="sxs-lookup"><span data-stu-id="c5491-128">Error codes</span></span>
<span data-ttu-id="c5491-129">この API では、標準の HTTP エラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c5491-129">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="c5491-130">さらに、次の表に記載されているカスタムのエラー コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c5491-130">In addition, it returns the custom error codes listed in the following table.</span></span>

|<span data-ttu-id="c5491-131">エラー コード</span><span class="sxs-lookup"><span data-stu-id="c5491-131">Error code</span></span>     | <span data-ttu-id="c5491-132">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="c5491-132">Error message</span></span>              |
|:--------------------| :---------------------|
| <span data-ttu-id="c5491-133">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c5491-133">400 BadRequest</span></span> | <span data-ttu-id="c5491-134">要求 Id は、Null にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="c5491-134">RequestId cannot be Null.</span></span> |
| <span data-ttu-id="c5491-135">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c5491-135">400 BadRequest</span></span> | <span data-ttu-id="c5491-136">要求 ID が見つからないと要求します。</span><span class="sxs-lookup"><span data-stu-id="c5491-136">Request with request ID not found.</span></span> |
| <span data-ttu-id="c5491-137">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="c5491-137">400 BadRequest</span></span> | <span data-ttu-id="c5491-138">キャンセルは、スケジュールおよび PendingApproval の状態でのみ実行できます。</span><span class="sxs-lookup"><span data-stu-id="c5491-138">Cancellation can be done only on status Scheduled and PendingApproval.</span></span> |
| <span data-ttu-id="c5491-139">403 許可されていません。</span><span class="sxs-lookup"><span data-stu-id="c5491-139">403 UnAuthorized</span></span> | <span data-ttu-id="c5491-140">依頼者がするには [キャンセル] の呼び出し、または見つかりません要求は許可されません。</span><span class="sxs-lookup"><span data-stu-id="c5491-140">Requester not allowed to make Cancel call or request not found.</span></span> |

## <a name="example"></a><span data-ttu-id="c5491-141">例</span><span class="sxs-lookup"><span data-stu-id="c5491-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5491-142">要求</span><span class="sxs-lookup"><span data-stu-id="c5491-142">Request</span></span>
<span data-ttu-id="c5491-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c5491-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_privilegedRoleAssignmentRequests"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests('7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee')/cancel
```

##### <a name="response"></a><span data-ttu-id="c5491-144">応答</span><span class="sxs-lookup"><span data-stu-id="c5491-144">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Cancel privilegedRoleAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignmentrequest-cancel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
