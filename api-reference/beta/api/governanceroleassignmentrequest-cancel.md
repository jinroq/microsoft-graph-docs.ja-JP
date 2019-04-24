---
title: governanceRoleAssignmentRequest のキャンセル
description: governanceRoleAssignmentRequest を取り消します。
localization_priority: Normal
ms.openlocfilehash: 0437051a3d2550da8a8fe3e9984214ff7c885e3a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467328"
---
# <a name="cancel-governanceroleassignmentrequest"></a><span data-ttu-id="92b1f-103">governanceRoleAssignmentRequest のキャンセル</span><span class="sxs-lookup"><span data-stu-id="92b1f-103">Cancel governanceRoleAssignmentRequest</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92b1f-104">[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)を取り消します。</span><span class="sxs-lookup"><span data-stu-id="92b1f-104">Cancel a [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="92b1f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="92b1f-105">Permissions</span></span>
<span data-ttu-id="92b1f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92b1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92b1f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92b1f-108">Permission type</span></span>      | <span data-ttu-id="92b1f-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="92b1f-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92b1f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92b1f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="92b1f-111">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="92b1f-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="92b1f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92b1f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92b1f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92b1f-113">Not supported.</span></span>    |
|<span data-ttu-id="92b1f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92b1f-114">Application</span></span> | <span data-ttu-id="92b1f-115">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="92b1f-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="92b1f-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="92b1f-116">Optional query parameters</span></span>
<span data-ttu-id="92b1f-117">このメソッドは、 [OData クエリパラメーター](/graph/query-parameters)をサポートし**ていません**。</span><span class="sxs-lookup"><span data-stu-id="92b1f-117">This method does **not** support [OData Query Parameters](/graph/query-parameters).</span></span>

### <a name="http-request"></a><span data-ttu-id="92b1f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92b1f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedAccess/azureResources/roleAssignmentRequests/{id}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="92b1f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92b1f-119">Request headers</span></span>
| <span data-ttu-id="92b1f-120">名前</span><span class="sxs-lookup"><span data-stu-id="92b1f-120">Name</span></span>       | <span data-ttu-id="92b1f-121">説明</span><span class="sxs-lookup"><span data-stu-id="92b1f-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="92b1f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92b1f-122">Authorization</span></span>  | <span data-ttu-id="92b1f-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="92b1f-123">Bearer {code}</span></span>|
| <span data-ttu-id="92b1f-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="92b1f-124">Content-type</span></span>  | <span data-ttu-id="92b1f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92b1f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92b1f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="92b1f-126">Request body</span></span>
<span data-ttu-id="92b1f-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="92b1f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92b1f-128">応答</span><span class="sxs-lookup"><span data-stu-id="92b1f-128">Response</span></span>
<span data-ttu-id="92b1f-p102">成功した場合、このメソッドは `204 NoContent` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="92b1f-p102">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="92b1f-131">エラー コード</span><span class="sxs-lookup"><span data-stu-id="92b1f-131">Error codes</span></span>
<span data-ttu-id="92b1f-132">この API は、HTTP コードの標準に従います。</span><span class="sxs-lookup"><span data-stu-id="92b1f-132">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="92b1f-133">それに加えて、カスタムエラーコードは以下のとおりです。</span><span class="sxs-lookup"><span data-stu-id="92b1f-133">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="92b1f-134">エラー コード</span><span class="sxs-lookup"><span data-stu-id="92b1f-134">Error code</span></span>     | <span data-ttu-id="92b1f-135">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="92b1f-135">Error message</span></span>              | <span data-ttu-id="92b1f-136">詳細</span><span class="sxs-lookup"><span data-stu-id="92b1f-136">Details</span></span> |
|:--------------------| :---------------------|:--------------------|
| <span data-ttu-id="92b1f-137">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="92b1f-137">400 BadRequest</span></span> | <span data-ttu-id="92b1f-138">RoleAssignmentRequestNotFound</span><span class="sxs-lookup"><span data-stu-id="92b1f-138">RoleAssignmentRequestNotFound</span></span> | <span data-ttu-id="92b1f-139">governanceRoleAssignmentRequest は、システムに存在しません。</span><span class="sxs-lookup"><span data-stu-id="92b1f-139">The governanceRoleAssignmentRequest does not exist in system.</span></span>
| <span data-ttu-id="92b1f-140">400 badrequest</span><span class="sxs-lookup"><span data-stu-id="92b1f-140">400 BadRequest</span></span> | <span data-ttu-id="92b1f-141">RequestCannotBeCancelled</span><span class="sxs-lookup"><span data-stu-id="92b1f-141">RequestCannotBeCancelled</span></span>    | <span data-ttu-id="92b1f-142">、 `Granted` `PendingApproval`、、の状態の要求のみ`PendingAdminDecision`を取り消すことができます。 `PendingApprovalProvisioning`</span><span class="sxs-lookup"><span data-stu-id="92b1f-142">Only requests in status of `Granted`, `PendingApproval`, `PendingApprovalProvisioning` and `PendingAdminDecision` can be cancelled.</span></span>

## <a name="example"></a><span data-ttu-id="92b1f-143">例</span><span class="sxs-lookup"><span data-stu-id="92b1f-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92b1f-144">要求</span><span class="sxs-lookup"><span data-stu-id="92b1f-144">Request</span></span>
<span data-ttu-id="92b1f-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="92b1f-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "cancel_governanceroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel
```

##### <a name="response"></a><span data-ttu-id="92b1f-146">応答</span><span class="sxs-lookup"><span data-stu-id="92b1f-146">Response</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Cancel governanceRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-cancel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
